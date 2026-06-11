---
layout: post
title: "Building My First Website with GitHub Pages (and the Mistakes I Made)"
date: 2026-06-11 10:30:00 -0000
categories: blog
---


![Screenshot of my finished GitHub Pages site](/assets/images/first_website.png)

I built a live website for free without touching any web development languages, messing around with HTTP servers, or paying for a domain.
This blog exists to document my journey learning computer science and cyber security. Although my background is technical, I'm writing for everyone: I'll keep jargon to a minimum so that readers from any background can follow along.

## How you can build your own website

## The "Subscribe via RSS" Link I Never Wrote
![Screenshot of the Subscribe via RSS](/assets/images/subrss.png)
Once the website was live, I noticed underneath my first post there was caption I never wrote: "Subscribe via RSS". After a few minuites of Googling to why there was this line of text on my website, I found an old GitHub fourm relating to this issue.
[GitHub Link to the Issue](https://github.com/jekyll/minima/issues/375)

One of the problems is how the current repository (where folders and files are organised) is made. home.html and _layouts folder was not created. Since the website did not download the Minima template to the GitHub repository, some critcial files that were important in formating the website were missing.

![Screenshot of the Repository without the home.html and _layout folder](/assets/images/repo_without_layouts.png)

My reasoning for not downloading the Minima template is due to Abstraction. In Computer Science Education, there is a concept called Computational Thinking. In simple terms, breaking down a problem into managable steps and problem solving. Abstraction is the process of removing irelevant details in order to solve a problem and since this post is aimed for the general audience, I want to minimise the amount of confusion to setting up a website.

[If you want to read more about Computational Thinking, here is a great paper written by Jeannette M. Wing](https://www.cs.cmu.edu/~15110-s13/Wing06-ct.pdf)

![Screenshot of Minima's GitHub Repository](/assets/images/minima_repo.png)