---
layout: post
title: Starting with Rails
published: true
---

One thing that really troubled me when trying to get my site to run on an actual live production, was understanding which gems and services etc. that were relevant for me. I found lots of tutorials and guides, but they always seemed to cover something that was slightly different than my setup.

This is an over view of the different parts that you need, when you want to run a Ruby on Rails application, and their different variants. The top most row is what I currently use.

Rack server | Web server | Database
----------- | ---------- | ----------
Unicorn     | Nginx      | PostgreSQL
Puma        | Apache     | MySQL
Passenger   |            | 
Thin        |            |
WEBrick*    |            | SQLite*

* These are for development

DISCLAIMER:
I'm writing this to understand it myself. If you see something that's clearly wrong, please let me know [@floede](https://twitter.com/floede)

The point is that if you read a guide that assumes you're using Passenger, but the server you have uses Unicorn, you'll know that these two handle the same tasks, and you'll only need one of them.


## Links

[ruby-toolbox.com/categories/web_servers](https://www.ruby-toolbox.com/categories/web_servers)

[stackoverflow.com/questions/4113299/ruby-on-rails-server-options](http://stackoverflow.com/questions/4113299/ruby-on-rails-server-options)