---
id: 719
title: 'Has Deep Learning Uncovered Chomsky&#8217;s Deep Structure?'
date: 2016-11-27T10:59:03-06:00
author: angoodkind
layout: post
guid: http://adamgoodkind.com/?p=719
permalink: /blog/has-deep-learning-uncovered-chomskys-deep-structure/
dsq_thread_id:
  - "5336160010"
categories:
  - Computational Linguistics
  - Linguistics
  - NLP
---
After Trump&#8217;s shocking victory, many of our professors began class with an opportunity for us to voice any fears or feelings we were harboring. One of my professors spoke about how studying linguistics is a way to study what unites us as humans: this strange ability called &#8220;language.&#8221; Despite all of our languages looking and sounding different, all humans have this amazing ability to learn complex rules and thousands of words in our first few years of existence. Moreover, we do this without being prodded to learn and without much explicit instruction. Language is something that should, at its core, unite us, not divide us.

Earlier this week,&nbsp;[Google Research announced a breakthrough in &#8220;one-shot&#8221; machine translation](https://research.googleblog.com/2016/11/zero-shot-translation-with-googles.html?m=1). What this means is that Google Translate can now perform translations on unseen pairs of languages. Typically, a machine translation algorithm needs to be trained on each language pair, e.g. English <&#8211;> French and French <&#8211;> Spanish. But Google&#8217;s latest results can perform translations from, e.g., English <&#8211;> Korean by only being trained on pairs of _other_ languages (see Google&#8217;s visual representation below). In essence, they are only training the machine on the &#8220;gist&#8221; of language or language relationships, rather than a specific pairing.

<img class="wp-image-718 alignnone size-full" src="http://adamgoodkind.com/wp-content/uploads/2016/11/wp-1480261428126.gif" alt="" width="800" height="423" /> 

The Google team calls this &#8220;[interlingua](https://arxiv.org/pdf/1611.04558v1.pdf).&#8221; For linguists, this underlying abstract form has been the basis of their field since Chomsky&#8217;s earliest writings. &#8220;Deep Structure&#8221; or D-structure, is distinct from &#8220;Surface Structure,&#8221; or S-structure; where Deep Structure is something like the Platonic form, the S-structure is the concrete realization in the phonetic sounds of a sentence. For example, the sentences _I love New York_ and _New York is loved by me_ both have essentially the same meaning. According to Chomsky, the D-structure of both of these sentences is the same, and the deep structure is transformed in different ways en route to the different respective surface realizations.&nbsp;

The field of generative syntax has been primarily concerned with elucidating the rules and constraints that each and all languages undergo during this transformational process. If we can unwind these transformations, peeling back layer upon layer of surface structure, then we can uncover the deep structure underlying all of language.

And now, it&#8217;s my turn to be speculative: For the last 20 years, computational linguists have been trying to apply the rules and constraints of generative syntax to the computational tasks of natural language understanding and translation. However, rules-based accounts have been less successful than the more flexible probability-based algorithms. The result has been that many &#8220;language engineers&#8221; have become dismissive of the rules-based Chomskian community.

But if we (speculatively) assume that Google&#8217;s algorithms have uncovered an underlying interlingua, then perhaps this means that Chomsky&#8217;s notion of D-structure has been right all along, we&#8217;ve just been going about the process of uncovering it in the wrong way. Whereas generative syntacticians base most of their findings on patterns in a single language or single collection of languages, maybe the real findings lie in the space between languages, the glue that binds it all together.

Of course, the findings of many deep learning-based systems are notoriously difficult to suss apart, so we don&#8217;t really know what the features of this possible interlingua look like. While this is frustrating, I suppose it also means there is still plenty of work left for a budding computational linguist. And if we can start to elucidate the ties that linguistically bind us, maybe we can elucidate the ties that bind humanity, as well.