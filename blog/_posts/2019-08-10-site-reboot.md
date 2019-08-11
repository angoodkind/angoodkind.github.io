---
layout: post
title: A shiny new adamgoodkind.com
subtitle: Like a Disney reboot, but good!
tags: [R, Jekyll, Github, Markdown, Website]
image: /img/hercules0.jpg
output:
  html_document:
    keep_md: true
---

### Intro

It's been a few years since I've updated my web presence, and things were scattered all over, from my personal website, to my academic website, to some posts on [medium](medium.com) and [reddit](reddit.com). Now it's time to call the whole family in for dinner, and gather everything together on my revamped homepage.

At the moment, there isn't much new here, but I thought that setting up this site was *way too easy*, in that I just forked a github repo, and had a really pretty site in less than 5 minutes. If you're also interested in something like this, here are a few pointers:

### 1. Use [`beautiful-jekyll`](https://github.com/daattali/beautiful-jekyll#readme)

The git repo this was forked from is called [`beautiful-jekyll`](https://github.com/daattali/beautiful-jekyll#readme). The template is really well documented, and very very easy to use. You can literally create your own `github.io` page in under 5 minutes. If you'd like to use a custom domain, the template's creator, Dean, also has [a great blog post](https://deanattali.com/2015/03/12/beautiful-jekyll-how-to-build-a-site-in-minutes) for how to set this up.

### 2. Using a custom domain (optional)

I will admit, I ran into some roadblocks with linking my github.io site to an already existing custom domain, and fell into a little rabbit hole trying to figure it out. (Note: This was not the fun kind of rabbit hole like in *Alice in Wonderland*.) I found [github's own documention](https://help.github.com/en/articles/using-a-custom-domain-with-github-pages) useful, if somewhat verbose. In addition, because my domain was already registered on Google Domains, I found [this blog post](https://medium.com/employbl/launch-a-website-with-a-custom-url-using-github-pages-and-google-domains-3dd8d90cc33b) and [this blog post](http://www.curtismlarson.com/blog/2015/04/12/github-pages-google-domains/) helpful, as well, for connecting one piece to the other.

My biggest takeaway from this is that, which I wish I knew beforehand: 
> <span style="font-family:Arial-black; font-size:1.5em">Changing something on the internet takes a bit longer than saving a file on your computer. You will probably need to wait 10-15 minutes for each change to propogate through the series of tubes that is the World Wide Web.</span>

### 3. Importing wordpress blog posts (optional)

A big part of my motivation to consolidate sites was the freedom available within my own domain, whether my custom domain or e.g., a github domain. I was really tired of all the limitations (and general ugliness) of wordpress. On top of this, Northwestern has its own flavor of wordpress, with higher walls and less options. (Don't get me wrong, I understand that they need to do this, so that all affiliated websites are guaranteed to be secure and shouldn't break anything downstream.)

I was pleasantly surprised to find that it's really easy to export wordpress blog posts to jekyll (which uses markdown). There are lots of tools available. I liked [this one](https://github.com/benbalter/wordpress-to-jekyll-exporter), and exported everything in 1 click. By and large, the resulting markdown files were formatted correctly, with an occassional broken link or image.

### 4. Using R markdown (optional)

I also really enjoy writing up tutorials and doing data visualization in `R`. As such, I really wanted the ability to write blog posts in [`R markdown`](https://rmarkdown.rstudio.com) rather than just vanilla `markdown`. Jacob Fiksel set up a great utility for this, along with [an easy to understand blog post](https://rmarkdown.rstudio.com). If you want to create blog posts in RStudio, with pretty charts, this is the route to go. To test this out, I rewrote [my last blog post about the books I read in 2017](https://adamgoodkind.com/2018-01-09-2017-in-books/). In general, it works really well, and was fun to use.

### Conclusion

This could not have been simpler. I am deeply indebted to all of the developers I linked to above, who helped me get over a lot of obstacles that I created myself, trying to mix pre-existing parts with new parts. If you're just getting started, though, this is a great way to jump in. 

Hopefully this will be the first post in a more regular series of posts going forward. 

<span style="color:blue">
L
</span>
<span style="color:orange">
F
</span>
<span style="color:blue">
G
</span>
<span style="color:orange">
M
</span>
!