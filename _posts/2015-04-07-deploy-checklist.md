---
published: false
---

# Deploy checklist
A list of commends to remember

## Start Vagrant Virtual Machine:
vagrant up
vagrant ssh

## Load SSH key:
exec ssh-agent bash
ssh-add

## Deploy:
cap production deploy

## On server stop and restart unicorn:
service unicorn stop
unicorn_rails -c config/unicorn.rb -D -E production

## Restart Nginx:
service nginx restart
