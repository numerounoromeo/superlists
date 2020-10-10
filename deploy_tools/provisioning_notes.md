Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3.8.5
* virtualenv + pip
* Git

eg, on Ubuntu:

    sudo apt-get install nginx git python38 python3.8-venv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, e.g., staging.my-domain.com

## Systemd service

* see gunicorn-systemd.template.service
* replace SITENAME with, e.g., staging.my-domain.com

## Folder structure:
Assume we have a user account at /home/username

/home/username
|__ sites
    |__ SITENAME
        |__ database
        |__ source
        |__ static
        |__ venv
     
