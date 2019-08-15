# Udacity Flask Catalog Web Application
A simple catalog web app developed as part of Udacity's Full-stack nanodegree.
The app uses Python's Flask framework and incorporates OAuth2 as an authorization method.
___
## Table of content
* Overview
* Requirements
* How to run the project?
* Known issues
___
## Overview
The aim of this task is to implement basic CRUD operations in a web application, more specific in a Sports Catalog.
It implements the Flask framework, together with SQLAlchemy. The task further uses Flask-SQLAlchemy as it implemets a pagination function. Furthermore, it implements a login system that uses OAuth2 by
allowing google and facebooh authentication. The Edit, Add and Delete operations are handled with AJAX requests and do not incorporate their own templates. The structure of the app is built with Bootstrap 4 and jQuery. The app structure is as follows:
```
|   client_secrets.json
|   database_setup.py
|   database_setup.pyc
|   db_population.py
|   fb_client_secrets.json
|   final-project.py
|   README.md
|   testDB.db
|
+---static
|   +---css
|   |       user_style.css
|   |
|   \---js
|           app.js
|
\---templates
        category-index_logged.html
        category-index_not_logged.html
        category-item-index_logged.html
        category-item-index_not_logged.html
        item-index_logged.html
        item-index_not_logged.html
        layout_logged.html
        layout_not_logged.html
        login.html
```
_____
## Requirements
* [Python3](https://www.python.org/downloads/release/python-374/) - OOP programming language
* [Vagrant](https://www.vagrantup.com/) - Builds the virtual environment
* [VirtualBox](https://www.virtualbox.org/) - VM virtualization
* [Git](https://git-scm.com/) - Version control
* [Bootstrap4](https://getbootstrap.com/docs/4.3/getting-started/download/) - framework for building responsive, mobile-first sites
* [jQuery](https://jquery.com/download/) - JavaScript library
* [Flask](https://github.com/pallets/flask) - Python MVC Framework
* [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/) - adds support for SQLAlchemy to your application
___

## How to run the project?
1. Install the latest version of Python from the [link](https://www.python.org/downloads/release/python-374/).
2. Download and install [VirtualBox](https://www.virtualbox.org/) and [Vagrant](https://www.vagrantup.com/).
3. Download Udacity's pre-configured [Vagrant file](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59822701_fsnd-virtual-machine/fsnd-virtual-machine.zip).
4. Clone this [repo](https://github.com/udacity/fullstack-nanodegree-vm).
5. Install Flask with `pip install -U Flask`.
6. Install Flask-SQLAlchemy with `pip install -U Flask-SQLAlchemy`.
7. After cloning the repo from step 4, navigate your terminal to the Udacity folder and type `cd /vagrant`.
8. Initialize the virtual machine with `vagrant up`.
9. After the install is complete, run `vagrant ssh` to connect to the VM. Your bash should now be under vagrant.
10. `cd /vagrant` to go into the project directory and look around.
11. `cd /catalag` to go into the web app application.
12. The first step is to to setup the database with `python db_setup.py`.
13. Afterwards, populate the database with `python db_population`. You will see a testDB.db file appear in the folder.
14. Run the applicaiton `python final_project.py`.
___
## Known issues
In order for the Google sign in button to work you need to delete your browser cache by pressing `Ctrl + F5`.
