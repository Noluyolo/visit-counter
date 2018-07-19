# Project Title

Repository implementation

# Description
Two core concepts are conveyed in the vanilla example: 1) how to build your own docker from Dockerfile, and 2) how to mount a volume inside of a docker.

# Prerequisites

Install apache , PHP, 
 Docker, 
mysqli and net-tools.

## Installing

https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04.

# Coding style tests

 git init
 git status
 touch file
 git add file
 git commit -m" "
 git log
 git pull origin master
 git push -u origin master

## run with docker image built from Dockerfile

docker run --rm \
  -p 80:80 \
  --name visit-counter \
  test/visit-counter

## run with official php docker image

docker run --rm \
  -p 80:80 \
  --name php \
  -v "$PWD/scripts":/var/www/html \
  php:7.0-apache

# How to overwrite the web root with a volume at runtime

docker run --rm \
  -p 80:80 \
  --name visit-counter \
  -v "$PWD/scripts":/var/www/html \
  test/visit-counter

# How to access

http://localhost/counter.php

 
 # Links
 
Here is the link for the hit counter that you can use: http://justintadlock.com/web-design/counter.

Docker image extended from https://hub.docker.com/_/php/
