---
layout: default
title: "How Jekyll works under the hood?"
date: 2023-02-27 07:18:00
categories: ruby
---

This blog was created using [Jekyll](https://jekyllrb.com/) and [Github Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll). It's a pretty cool feature that Github made available and it's a great tool in Ruby ecosystem and community.

As described in Jekyll's documentation, Jekyll takes Markdown and HTML files and creates a complete static website based on your choice of layouts. That's the magic that makes it so simple and yet powerful. Although they say Jekyll has no "magic" in their [philosophy](https://jekyllrb.com/philosophy/) page. Maybe a tip for Rails?


But I wondered how it really works under the hood? I decided to take a look and add this learning in my skillset.

Everything starts with the file structure, with consists in basically in *pages*, *posts* and *assets* which will contain all the necessary styling and other resources such as images, icons, videos, etc.

After that the command `jekyll build` is responsible to turn all the files created in markdown files in a static website. To understand better this command, let's take a look at Jekyll's [main repository](https://github.com/jekyll/jekyll)








