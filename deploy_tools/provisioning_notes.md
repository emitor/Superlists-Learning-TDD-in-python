Provisioning a new site
=======================

## Required Packages

*nginx
*Python 3.6
*virtualenv + pip
*Git

e.g. on Ubuntu 18.04 LTS:

	sudo apt update
	sudo apt upgrade
	sudo apt install nginx git python3 python3-venv 

## NGINX Virtual host config

* see nginx.template.conf
* replace DOMAIN with, e.g., staging.mydomain.com

## Folder structure:

Assume we have a user account at /home/username

/home/username
└── sites
	├── DOMAIN1
	|	├── .env
	|	├── db.sqlite3
	|	├── manage.py
	|	├── ...(etc)
	|	├── static
	|	└── virtualenv
	├── DOMAIN2
	|	├── .env
	|	├── db.sqlite3
	|	├── manage.py
	|	├── ...(etc)
	|	├── static
	|	└── virtualenv
	(...)

