---
title: "Build a similar Website!"
last_modified_at: 2022-09-06T16:20:02-05:00
categories:
  - Blog
tags:
  - Jekyll
  - Ruby
  - GitHub
  - Web

excerpt : "How to build a similar website with Jekyll, Ruby and Remote theme."
---

# Welcome to Batteries Included!

Around here you will find content about Data Science in general and especially Machine Learning and Data Visualization. 

Check out the [About Me]({% link _pages/about.md %}) to discover more about me! 

This site has been build using Jekyll and a great theme called [Minimal-Mistakes](https://mmistakes.github.io/minimal-mistakes/). 

## How to build a similar website

### 1. Install Ruby and Jekyll on your machine

This is pretty straightforward, in order to develop your website you will need to install both of them. 

You can check out the following Youtube playlist for Jekyll Installation and Basic configuration : 

{% include video id="T1itpPvFWHI" provider="youtube" %}

Then, I simple created a first project using : 

```python
jekyll new
```

### 2. Use the remote theme and customize it 

I have chosen a theme called [Minimal-Mistakes](https://mmistakes.github.io/minimal-mistakes/). As the website is hosted on GitHub Pages, it seems better to use a remote theme, acording to the theme [documentation](https://mmistakes.github.io/minimal-mistakes/docs/installation/).

A good way to experiment with the theme is to first use the [remote theme starter](https://github.com/mmistakes/mm-github-pages-starter/generate). 

If you are a more advanced user of Jekyll, you can fork the [theme repository](https://github.com/mmistakes/minimal-mistakes) and completely edit it. 

As for me, my strategy was to use the the remote theme method but to clone the theme repository and grab files I would need to edit. Layouts, for exemple. 
Jekyll will use your local files as default and then use the remote theme files, so you can make minor changes this way. 

### 3. Host your Website on GitHub Pages 

This is a very simple way to host a website such as this one. 

Check it out [there!](https://pages.github.com/) 







