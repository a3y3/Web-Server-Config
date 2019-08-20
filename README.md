# Web-Server-Config
### What is this?
This file serves to display information about the linux machine that ~~hosts~~ hosted [Katalog](https://github.com/a3y3/Katalog).
The server is no longer up. Read on for information on how the server was configured.

### Warning
This repository contains a private key in plain text. This is meant only for the eyes of a Udacity grader. Please do not use this key if you are not a Udacity grader. For security purposes, the grader account for which the key is used will be deleted as soon as Udacity is done with this. 


## Server Information
### IP Address
The server is up at 54.226.36.197. 
### URL 
You can visit the server IP address to use the app. However, for signing in and using user features, you should use [54.226.36.197.xip.io](http://54.226.36.197.xip.io/). 
### Summary of software installed
- Apache2
- mod_wsgi
- Python3
- Postgresql
- pip3 install -r requirements.txt. [`requirements.txt` can be found [here](https://github.com/a3y3/Katalog).]
### Summary of configurations made
- Updated all currently installed packages.
- Enabled SSH logins for deafult account and grader account
- Changed the SSH port from 22 to 2200.
- Configured the firewall (UFW) to only allow incoming connections for SSH, HTTP, and NTP.
- Installed and configured mod_wsgi to serve Katalog on port 80.
- Provided limited access to the psql database for user www-data (Apache user)

## Private key
- See the file called 'graders' in root for the private key. 
- Use `ssh -i graders grader@54.226.36.197 -p 2200` for logging in.

### Third party resources used
- Stack Exchange (Stackoverflow, Serverfault, etc.)
- Flask documentation on [mod_wsgi](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/)
- [DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-tune-your-ssh-daemon-configuration-on-a-linux-vps)
