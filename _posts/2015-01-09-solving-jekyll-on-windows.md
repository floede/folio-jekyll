---
layout: post
title: Solving Jekyll for GitHub pages on Windows
published: true
---

Trying to work with Ruby (on Rails) on Windows is often a pain in the neck. So much so that I'm actually running Linux through Vagrant on my home computer.

But setting up this very blog couldn't require much I thought. I was so wrong.

With Jekyll you're encouraged to install the gem locally, and run a local Jekyll server to write and test your pages.

I followed the instructions from [juthilo](http://jekyll-windows.juthilo.com/), this was working fine for me, but I just couldn't get the files to build properly, once I pushed them to my GitHub repository. Even though I changed nothing in the original files that comes with Poole and Hyde, and I could run it locally just fine, I kept getting errors from GitHub.

Then I found this guide from [Eric Trinh](http://erictrinh.com/blog/jekyll-and-gh-pages/) detailing how you should aim to replicate GiHub's setup locally. This meant manually installing a ton of gems. Luckily Ruby tells you which and how.

However I kept getting errors that Jekyll couldn't load the syntax highlighter Rouge. 
> cannot load such file -- rouge 

I tried  re-installing and updating. Nothing helped.
Finally I caved in, and tried the other highlighter mentioned by juthilo  . Which required me to install Python. Working with modern web applications often feel like jumping into the rabbit hole. One gem requires another gem which leads to a third, and so on. Same goes for node packages really.

But after installing Python, and switching to Pygments, I was finally able to make it work. And you're able to read this.


## Links
[http://jekyll-windows.juthilo.com/](jekyll-windows.juthilo.com)

[http://erictrinh.com/blog/jekyll-and-gh-pages/](erictrinh.com/blog/jekyll-and-gh-pages)