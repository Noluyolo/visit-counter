# Project Title
Repository implementation

# Prerequisites

Install apache , PHP, 
 Docker, 
mysqli and net-tools.

## Installing

https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04.

# Coding style tests

I created repository > visit-counter.
Switch from home direction to repository > cd visit-counter.
Initialize this repository with README.md.
Git commit " ".
Add files (counter.php , countlog.txt 'put a (0) in it') > git touch filename ; gedit filename.
Remote add origin > https://github.com/username/repo.git.
Clone repo > SSH >git clone git@github.com:username/repo.git.
Push to origin master > git push -u origin master.

If the above command gives you an error, try this sudo /etc/init.d/apache2 stop.
And if still gives an error > docker rm php , try again and it should be successful.
sudo apt 
Build an image on docker > docker build -t anyname/php:name-1.0.0.0.
   vi dockerfile ; cat dockerfile (insert text); docker exec -ti php bash.
 chmod 777 counter.php ; chmod 777 countlog.txt - gives permissions
 
 # Links
 
Here is the link for the hit counter that you can use: http://justintadlock.com/web-design/counter.

Docker image extended from https://hub.docker.com/_/php/
