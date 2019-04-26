# Udacity Linux Server Configuration Project
This project involves configuration for a Linux Ubuntu box hosted on Amazon Lightsail.  This setup is configured to run an Apache 2.4.18 web server, and host a data-driven web application using Flask.  This project was completed as part of the **_Udacity Full Stack Nanodegree Course_**

## Ubuntu Linux Instance Information
The Ubuntu instance is hosted on Amazon Lightsail.  Details about this instance follow.
* Public IP Address `3.80.67.155`, SSH Port `2200`
* URL to the Hosted Flask Application `http://3.80.67.155/myApp/`

## Software Installed
Additional software required to complete this project needed to be installed to the Ubuntu instance.  The following were installed from the Linux Distrubutions using `sudo apt-get install` at a shell terminal prompt.
* Apache 2.4.18
* Mod_WSGI package for Apache
* PostgreSQL 9.5
* Git
* Python 3.5.2
* Pip
* Psycopg2

## Ubuntu Configuration Changes
* Changed SSH Port from 22 to 2200 in the Lighsail Console
* Configured UFW Firewall to only allow incomming connections for SSH, HTTP, and NTP
* Added an additional Unix user with `sudo` access privileges
* Added an alias to the **_~/.bashrc_** file: `alias python=python3` to use Python3 version when typing commands instead of the default Python 2.7 installation provided by Ubuntu.


## Third-Party Resources Used
The following list identifies the third-party web resources I used to complete this project.

### APAHCE CONFIGURATION
* [DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-configure-the-apache-web-server-on-an-ubuntu-or-debian-vps)
* [Mod-wsgi](https://modwsgi.readthedocs.io/en/develop/user-guides/quick-configuration-guide.html?highlight=VirtualHost)
* [Simon Jakowicz](https://www.jakowicz.com/flask-apache-wsgi/)
* [Flask-mod-wsgi](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/)
* [Daniel Abrao Github](https://github.com/jungleBadger/-nanodegree-linux-server-troubleshoot/blob/master/Blocked_SSH_port/README.md)
* [be Groovie](https://be.groovie.org/2005/10/07/wsgi_and_wsgi_middleware_is_easy.html)

### FLASK & POSTGRESQL CONFIGURATION
* [Theodo Blog](https://blog.theodo.com/2017/03/developping-a-flask-web-app-with-a-postresql-database-making-all-the-possible-errors/)
* [PostgreSQL 9.5](https://www.postgresql.org/docs/9.5/index.html)

## Created By
* Completed By: Jon Lunsford
* Date: April 25, 2019
* License: N/A


