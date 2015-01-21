---
layout: post
title: Starting with Rails
published: true
---

One thing that really troubled me when trying to get my site to run on an actual live production, was understanding which gems and services etc. that were relevant for me. I found lots of tutorials and guides, but they always seemed to cover something that was slightly different than my setup.

This is an over view of the different parts that you need, when you want to run a Ruby on Rails application.

Rack server | Web server | Database
----------- | ---------- | ----------
Unicorn     | Nginx      | PostgreSQL
Puma        | Apache     | MySQL
Passenger   |            | 
Thin        |            |
WEBrick*    |            | SQLite*


## Links

https://www.ruby-toolbox.com/categories/web_servers

http://stackoverflow.com/questions/4113299/ruby-on-rails-server-options