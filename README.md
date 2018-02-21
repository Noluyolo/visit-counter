I installed apache and PHP: https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04.
Here is the code for the hit counter that we are going to use: http://justintadlock.com/web-design/counter.
I creeated repository > visit-counter.
Switch from home direction to repository > cd visit-counter.
Initialize this repository with README.md.
Git commit " ".
Add files (counter.php , countlog.txt 'put a (0) in it') > git touch filename ; gedit filename.
Remote add origin > https://github.com/username/repo.git.
Clone repo > SSH >git clone git@github.com:username/repo.git.
Push to origin master > git push -u origin master.

 I installed Docker and then entered this command > docker run -dti -p 80:80 --name php -v "$PWD":/var/www/html php:7.0-apache.
If the above command gives you an error, try this sudo /etc/init.d/apache2 stop.
And if still gives an error > docker rm php , try again and it should be successful.
sudo apt install net-tools.
Build an image on docker > docker build -t anyname/php:name-1.0.0.0.
 vi dockerfile ; cat dockerfile (insert text); docker exec -ti php bash
