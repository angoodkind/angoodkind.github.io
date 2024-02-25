---
layout: post
published: true
title: A broken llama (index)!
# subtitle: but that doesn't matter...
tags: [AI, Chatbot]
image: /img/broken-llama.png
output:
  html_document:
    keep_md: true
---

<img align="right" src="/img/broken-llama.png" alt="A cartton llama with a jagged break down the middle" style="width:30%">

I'm trying to get better about writing more regularly, and part of this means writing shorter, less polished articles, rather than long articles that are well-formatted and punchy. I'm also trying to get better about sharing my findings when I figure out a bug, in the hopes that a) someone else will find it on Google and save themselves *n* hours,and b) I don't forget what I did, and waste *n+1* hours again.

I'm currently building a chatbot for my dissertation ([Theo The Thesis](https://theo-the-thesis.streamlit.app/)), which is useful for a) brushing up on my LLM skillset, and b) making the information in my thesis understandable to a broader audience.

But for now, I want to dive into a bug I encountered that there aren't many posts about on the internet (read: StackOverflow questions). My chatbot uses a lot of [LlamaIndex](https://docs.llamaindex.ai/en/stable/) functions, because the framework is flexible and allows easy integrations with **a lot** of other models, like OpenAI's or Amazon's. And a lot of tutorials us LlamaIndex to let you quickly setup a chatbot with just a few lines of code.

I started my chatbot with this extremely helpful blog post on the Streamlit site, [Build a chatbot with custom data sources, powered by LlamaIndex](https://blog.streamlit.io/build-a-chatbot-with-custom-data-sources-powered-by-llamaindex/). It uses the following imports:

```python
import streamlit as st
from llama_index import VectorStoreIndex, ServiceContext, Document
from llama_index.llms import OpenAI
import openai
from llama_index import SimpleDirectoryReader
```
But all of a sudden my chatbot, which had been working well for a couple months, started throwing errors that looked like this:
```
ImportError: This app has encountered an error. The original error message is redacted to prevent data leaks. Full error details have been recorded in the logs (if you're on Streamlit Cloud, click on 'Manage app' in the lower right of your app).
Traceback:
File "/home/adminuser/venv/lib/python3.9/site-packages/streamlit/runtime/scriptrunner/script_runner.py", line 535, in _run_script
    exec(code, module.__dict__)
File "/mount/src/llamaindex-chat-with-streamlit-docs/streamlit_app.py", line 2, in <module>
    from llama_index import VectorStoreIndex, ServiceContext, Document
``` 

It turns out that when LlamaIndex [rolled out version 0.10 on February 12, 2024](https://blog.llamaindex.ai/llamaindex-v0-10-838e735948f8), it broke a lot of these import structures. Those same imports above will now look like this:

```python
import streamlit as st
from llama_index.core.indices.vector_store.base import VectorStoreIndex
from llama_index.core.indices.service_context import ServiceContext
from llama_index.llms.openai import OpenAI
from llama_index.core import SimpleDirectoryReader

## some other libraries I'm now using
from llama_index.core.indices.prompt_helper import PromptHelper
from llama_index.embeddings.openai import OpenAIEmbedding
from llama_index.core.node_parser import SentenceSplitter
```
My code was working fine when I served it locally, but was not working when I tried using the Streamlit Community Cloud or 
Github's Codespaces. This didn't make sense because I recently re-installed Streamlit. From what I can tell, if `pip` finds an older version of a package on your computer, it will just reuse that. Even though I had uninstalled and reinstalled `streamlit`, an old version of `llamaindex` was still lurking around. I would get messages saying that the requirement was already satisfied, seemingly regardless of what I tried removing from my computer. On the other hand, streamlit and codespaces was using the newest version of llamaindex, which is why my code didn't work on the remote server.

Anyway, there haven't been a lot of streamlit + llamaindex tutorials written since February 12 (2 weeks ago, as of this writing). I will be writing one, but in the meantime just be aware of these breaking changes, and make sure you update streamlit and llamaindex on your local machine.