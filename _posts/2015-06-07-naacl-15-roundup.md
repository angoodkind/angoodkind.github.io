---
id: 561
title: 'NAACL &#8217;15 Roundup'
date: 2015-06-07T14:01:40-06:00
author: angoodkind
layout: post
guid: http://adamgoodkind.com/?p=561
permalink: /blog/naacl-15-roundup/
dsq_thread_id:
  - "3906820058"
categories:
  - Academia
  - CART
  - Computational Linguistics
  - NLP
---
<img class="alignright" src="https://lh3.googleusercontent.com/VdlNPthrgylUP3zRLHKvfzDbxwViPpRi8TePbOeu3h8=w984-h769-no" alt="" width="286" height="224" />

I just returned from [NAACL 2015](http://naacl.org/naacl-hlt-2015/) in beautiful Denver, CO. This was my first &#8220;big&#8221; conference, so I didn&#8217;t know quite what to expect. Needless to say, I was blown away (for better or for worse).

First, a side note: I&#8217;d like to thank the NAACL and specifically the conference chair [Rada Mihalcea](http://web.eecs.umich.edu/~mihalcea/) for providing captions during the entirety of the conference. Although there were some technical hiccups, we all got through them. Moreover, [Hal Daume](http://www.umiacs.umd.edu/~hal/) and the rest of the NAACL board were extrememly receptive to expanding accessibility going forward. I look forward to working with all of them.

Since this was my first &#8220;big&#8221; conference, this is also my first &#8220;big&#8221; conference writeup. Let&#8217;s see how it goes.

<img class="aligncenter" src="https://lh3.googleusercontent.com/bYh64VdmTIXemY9LTHRxXWRB9lpNhW0w_vM3Jn7hAJQ=w1164-h372-no" alt="Packed ballroom for keynote" width="1164" height="372" /> 

<span style="text-decoration: underline;">Keynote #1: Lillian Lee <em>Big Data Pragmatics etc&#8230;.</em></span>

  * This was a really fun and insightful talk to open the conference. There were a few themes within Lillian&#8217;s talk, but my two favorite were why movie quotes become popular and why we use hedging. Regarding the first topic, my favorite quote was: _**&#8220;When Arnold says, &#8216;I&#8217;ll be back&#8217;, everyone talked about it. When I say &#8216;I&#8217;ll be back&#8217;, you guys are like &#8216;Well, don&#8217;t rush!'&#8221;**_

  * The other theme I really enjoyed was &#8220;hedging&#8221; and why we do it. I find this topic fascinating, since it&#8217;s all around us. For instance, in saying &#8220;_I&#8217;d claim_ it&#8217;s 200 yards away&#8221; we add no new information with _I&#8217;d claim_.&#8221; So why do we say it? I think this is also a hallmark of hipster-speak, e.g. &#8220;This is maybe the best bacon I&#8217;ve ever had.&#8221;

[<span style="text-decoration: underline;">Ehsan Mohammady Ardehaly & Aron Culotta <em>Inferring latent attributes of Twitter users with label regularization</em></span>](http://www.aclweb.org/anthology/N15-1019)

  * This paper uses a lightly-supervised method to infer attributes like age and political orientation. It therefore avoids the need for costly annotation. One way that they infer attributes is by determining which Twitter accounts are central to a certain class. Really interesting, and I need to read the paper in-depth to fully understand it.

<span style="text-decoration: underline;">One Minute Madness</span>

  * This was fun. Everyone who presented a poster had one minute to preview/explain their poster. Some &#8220;presentations&#8221; were funny and some really pushed the 60-second mark. [Joel Tetreault](http://www.cs.rochester.edu/~tetreaul/academic.html) did a nice job enforcing the time limit. Here&#8217;s a picture of the &#8220;lineup&#8221; of speakers.

<img class="aligncenter" src="https://lh3.googleusercontent.com/2b4kyXxF10GVG_2AcwLoAPoYUdIc8N0Mh0HMRGOE7uU=w1164-h419-no" alt="Long line of speakers" width="1164" height="418" /> 

[<span style="text-decoration: underline;">Nathan Schneider & Noah Smith <em>A Corpus and Model Integrating Multiword Expressions and Supersenses</em></span>](http://www.aclweb.org/anthology/N15-1177)

  * Nathan Schneider has been doing some really interesting semantic work, whether on FrameNet or MWEs. Here, the CMU folks did a ton of manual annotation of the &#8220;supersense&#8221; of words and MWEs. Not only do they manage to achieve some really impressive results on tagging of MWES, but they also have provided a really valuable resource to the MWE community in the form of their **[STREUSLE 2.0](http://www.ark.cs.cmu.edu/LexSem/)** corpus of annotated MWEs/supersenses.

<span style="text-decoration: underline;">Keynote #2: Fei-Fei Li <em>A Quest for Visual Intelligence in Computers</em></span>

  * This was a fascinating talk. The idea here is to combine image recognition with semantics/NLP. For a computer to really &#8220;identify&#8221; something, it has to understand its meaning; pixel values are not &#8220;meaning.&#8221; I wish I had taken better notes, but Fei-Fei&#8217;s lab was able to achieve some incredibly impressive results. Of course, even the best image recognition makes some (adorable) mistakes.

<div style="width: 1033px" class="wp-caption aligncenter">
  <a href="https://twitter.com/AppleBallCar/status/606252241494753280"><img class="" src="https://pbs.twimg.com/media/CGnXMwNUAAAdji3.jpg:large" alt="baby holding a toothbrush is mislabelled as " width="1023" height="854" /></a>
  
  <p class="wp-caption-text">
    Middle caption: &#8220;a young boy is holding a baseball bat&#8221;
  </p>
</div>

[<span style="text-decoration: underline;">Manaal Faruqui et al. <em>Retrofitting Word Vectors to Semantic Lexicons</em></span>](http://www.aclweb.org/anthology/N15-1184)

  * This was one of the papers that won a Best Paper Award, and for good reason. It addresses a fundamental conflict in computational linguistics, specifically within computational semantics: distributional meaning representation vs. lexical semantics. The authors combine distributional vector representation with information from lexicons such as WordNet and FrameNet, and achieve significantly higher accuracy in semantic evaluation tasks from multiple languages. Moreover, their methods are highly modular, and they have made their tools [available online](https://github.com/mfaruqui/retrofitting). This is something I look forward to tinkering around with.

<span style="text-decoration: underline;">Some posters that I really enjoyed</span>

  * [_Oracle and Human Baselines for Native Language Identification_ &#8211; Shervin Malmasi, Joel Tetreault and Mark Dras](http://www.aclweb.org/anthology/W15-0620)
  * [_Lexicon-Free Conversational Speech Recognition with Neural Networks_ &#8211; Andrew L. Maas, Ziang Xie, Dan Jurafsky, Andrew Y. Ng](http://www.aclweb.org/anthology/N15-1038)
  * [_Using Zero-Resource Spoken Term Discovery for Ranked Retrieval_ &#8211; Jerome White et al.](http://www.aclweb.org/anthology/N15-1061)
  * [_Recognizing Textual Entailment using Dependency Analysis and Machine Learning_ &#8211; Nidhi Sharma, Richa Sharma and Kanad K. Biswas](http://www.aclweb.org/anthology/N15-2020)

<span style="text-decoration: underline;">Overall impressions</span>

  * Deep learning and neural nets are still breaking new ground in NLP. If you&#8217;re in the NLP domain, it would behoove you to gain a solid understanding of them, because they can achieve some incredibly impressive results.
  * Word embeddings: The running joke throughout the conference was that if you wanted your paper to be accepted, it had to include &#8220;word embeddings&#8221; in the title. Embeddings were everywhere (I think I saw somewhere that ~30% of the posters included this is their title). Even Chris Manning felt the need to comment on this in his talk/on Twitter:

<blockquote class="twitter-tweet" lang="en">
  <p dir="ltr" lang="en">
    RT <a href="https://twitter.com/aidotech">@aidotech</a>: RT aidotech: Chris actually showing a tweet on his slides! <a href="https://twitter.com/hashtag/deeplearning?src=hash">#deeplearning</a> <a href="https://twitter.com/hashtag/naacl2015?src=hash">#naacl2015</a> <a href="http://t.co/GWI7rDiQVC">pic.twitter.com/GWI7rDiQVC</a>
  </p>
  
  <p>
    — StanfordCSLI (@StanfordCSLI) <a href="https://twitter.com/StanfordCSLI/status/606955070400413696">June 5, 2015</a>
  </p>
</blockquote>



<span style="text-decoration: underline;">Takeaways for Future Conferences</span>

  * I should&#8217;ve read more of the papers beforehand. Then I would have been better prepared to ask good questions and get more out of the presentations.
  * As Andrew warned me beforehand &#8220;You will burn out.&#8221; And he was right. There&#8217;s no way to fully absorb every paper at every talk you attend. At some point, it becomes beneficial to just take a breather and do nothing. I did this Wednesday morning, and I&#8217;m really glad I did it.
  * Get to breakfast early. If you come downstairs 10 minutes before the first session, you&#8217;ll be scraping the (literal) bottom of the barrel on the buffet line.

Shameless self-citation: [Here](http://www.aclweb.org/anthology/W15-0914) is the paper Andrew and I wrote for the conference.