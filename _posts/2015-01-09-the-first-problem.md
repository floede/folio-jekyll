---
layout: post
title: Very first problem
---

Strangely `jekyll serve` makes the server crash. No errors.

I'm writing this on Windows 7. While not recommended, I'm taking my chances and I've had no problems as such setting up Jekyll on this machine.

However today, the local server just stops working.

After reading a couple of StackOverflow posts, I tried downgrading to Jekyll 2.1.1.
It solved the problem, but also removed the "watch" feature, which I quite like from Grunt.

Tried running `jekyll serve --watch` and the problem returned.

So apparently there's some problem with the watch task - probably because I'm on Windows.