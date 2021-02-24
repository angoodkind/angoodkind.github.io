---
layout: page
title: Research
subtitle: Current and past research projects, with some relevant links
---

## Current Projects

__Human Behavior When Interacting With a Chatbot or Another Person__

This research uses keystroke-production data as a way to understand human-computer interaction at a deeper level. In many ways, keystroke productions parallels speech production, and has its own prosody and error correction. By looking at keystroke timing during discourse, we can better understand underlying cognitive processes and optimize interfaces and agents to maximize collaborative success.

Among other investigations, we focus on these research questions:
* How does anomalous behavior, such as a prolonger pause or a mistake, from a conversational partner affect a user's impression of their partner? Does it matter if their partner is a computer or another 
person?
* When we imitate our conversational partner (linguistic alignment), do we use the same cognitive resources to produce aligned text as we use when producing original text?
* Does a user's impression of their partner, especially whether they are another person or a computer, affect their overall typing production and ways of interacting?


## Past Projects
__Linguistics and Autism__

* Converting clinical transcripts into word vectors, we analyze semantic similarity in both typically-developing children (TD) and children with autism spectrum disorder (ASD). Our initial findings show that the cosine differences between children with ASD and TD children are significantly different when compared to a gold standard
  * [Goodkind, et al. (2018) Detecting Language Impairments in Autism: A Computational Analysis of Semi-structured Conversations with Vector Semantics](https://scholarworks.umass.edu/cgi/viewcontent.cgi?referer=&httpsredir=1&article=1006&context=scil)
  * [Code repository](https://github.com/angoodkind/vectoraut)

__Using Language Models to Understand Cognition__

* Do better language models better predict cognitive processes measured by eye-tracking? Using a neural net-based language model, we use generalized additive models (GAMs) to investigate how language models with lower perplexity can better model eye-tracking data. We are also investigating the distinct influence of lower-level (local) statistics such as transitional probability versus surprisal’s effects on processing.
  * [Goodkind, A. & Bicknell, K. (2018) Predictive power of word surprisal for reading times is a linear function of language model quality](https://www.aclweb.org/anthology/W18-0102) __(Best Paper Award)__
  * [Code repository](https://github.com/langcomp/lm_1b)

__Keystroke Dynamics__
* Typing patterns are unique to individuals. Just as everyone has a unique voice, such as pitch, rate of speech, and vocabulary, everyone has a unique way of typing. We frame typing patterns by the keystroke's linguistic context, such as the word within which the keystroke was produced, or that word's lexical category. For example, a typist might produce <em>TH</em> differently in a noun versus in a verb.
<br>We utilize keystroke dynamics for two tasks: individual identification and cohort identification. The first task uses keystroke dynamics to better identify an individual. The latter task uses keystroke dynamics to try to predict a typist's demographics, e.g. native language or gender, from their typing patterns.<br>
  * [Goodkind, A., Brizan, D. G., & Rosenberg, A. (2017). Utilizing overt and latent linguistic structure to improve keystroke-based authentication. Image and Vision Computing, 58, 230-238.](https://www.sciencedirect.com/science/article/pii/S0262885616301019)

* I'm also interested in how best to visualize keystroke data. The paper below is a dashboard I created for researchers. For my thesis, I am also interested in how keystroke data can best be shared with a conversational partner, to improve the conversation. For example, if keystroke patterns imply that a user is confused, then perhaps the speaker should re-explain what they are saying.
  * [Goodkind, A. (In Submission). TypeShift: A User Interface for Visualizing the Typing Production Process.](angoodkind.github.io/files/ACL_2020_TypeShift_System_Demo-2.pdf)
* Some questions that still vex me:
  * How do temporal patterns surrounding typing reflect cognition and language familiarity?
  * Why do we pause in the midst of typing?
  * Do certain linguistic phenomena induce pauses in typing?

__Multi-word Expressions__
* Multi-word expressions (MWEs) are phrases such as "kick the bucket" or "a lot" which are made up of multiple words but are single lexical units. I study how we store and retrieve these types of lexical units in working memory. According to current hypotheses, MWEs are stored as a single unit, rather than word by word. My current research investigates how this is realized during language output, specifically typed text.
  * [Goodkind, A., & Rosenberg, A. (2015). Muddying the multiword expression waters: How cognitive demand affects multiword expression production. In Proceedings of the 11th Workshop on Multiword Expressions.](https://www.aclweb.org/anthology/W15-0914)


## Resources
* [How to write a great research paper](https://www.youtube.com/watch?time_continue=786&v=VK51E3gHENc)
  * My own LaTeX template inspired by this incredible talk: https://github.com/angoodkind/paper_inspiration
