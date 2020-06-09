---
layout: post
title: Testing my Capistrano deploy
published: true
---


config.serve_static_files configures Rails itself to serve static files. Defaults to true, but in the production environment is turned off as the server software (e.g. NGINX or Apache) used to run the application should serve static assets instead. Unlike the default setting set this to true when running (absolutely not recommended!) or testing your app in production mode using WEBrick. Otherwise you won't be able use page caching and requests for files that exist regularly under the public directory will anyway hit your Rails app.


## Links

[guides.rubyonrails.org](http://guides.rubyonrails.org/configuring.html#rails-general-configuration)