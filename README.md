# Udacity Linux Server Configuration project

This project involved configuring an Ubuntu web application server
and deploying a Python web application onto it.

## Server info

IP address: 18.233.96.244
SSH port: 2220

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
Configured the `/etc/apache2/sites-enabled/000-default.conf` file.