# Udacity Linux Server Configuration project

This project involved configuring an Ubuntu web application server
and deploying a Python web application onto it.

## Server info

IP address: 18.233.96.244
SSH port: 2200

Web application url: http://18.233.96.244.xip.io/

## Installed software

postgresql
flask
sqlalchemy
flask_sqlalchemy
oauth2client
httplib2
requests
libapache2-mod-wsgi-py3
finger

## Configuration changes
Updated all installed packages.
Set up SSH to listen on port 2200. Set up firewall to only accept
connections on ports 80, 123 and 2200. Created Linux user "grader" with
sudo ability and SSH key pair. Created "catalog" database and postgresql
user "catalog". Deployed item catalog python 3 application, and made a few
changes for db connection. Added xip url to Google oauth authorized urls.
Configured the `/etc/apache2/sites-enabled/000-default.conf` file. Disabled
SSH login for root user.

## Third party resources used
1) Digital Ocean articles on [postgresql](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04), 
[SSH configuration](https://www.digitalocean.com/community/tutorials/how-to-tune-your-ssh-daemon-configuration-on-a-linux-vps) 
and [Flask](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)

2) [Blog post](http://terokarvinen.com/2016/deploy-flask-python3-on-apache2-ubuntu) 
on Flask/ Ubuntu/ wsgi

3) [Other blog post](https://jackhalpinblog.wordpress.com/2016/08/27/getting-your-python-3-flask-app-to-run-on-apache/) on Flask/ Ubuntu/ wsgi

4) Udacity forum

5) Stack Overflow