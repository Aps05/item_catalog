# Udacity Full-Stack Nanodegree
## Project 3 : Item Catalog
### by Apostolos Stephanou

## Overview

This project implements a list of categories and items in the form of restaurants and menu items and provides both html and json endpoints to be used by customers and third party software alike. It also implements third party authentication and authorization.

## How to Run

This project runs on a vagrant virtual machine. Please ensure you have the latest virtual box and vagrant versions installed for your operating system.

### Requirements

* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)

### Starting the VM

Navigate your terminal or command prompt to the project directory and run the following commands to connect to the virtual machine:
```bash
$ vagrant up
$ vagrant ssh
```

### Starting the server

Once connected to the VM, run the following to start the web server:
```bash
$ cd /vagrant
$ python project.py
```

Open your browser and navigate to localhost:5000.

## API Endpoints

Apart from a user friendly html interface this application also provides API endpoints to be used by other applications.
The endpoints are as follow:

* "localhost:5000/restaurant/JSON" - Retrieves all restaurants
* "localhost:5000/restaurant/<int:restaurant_id>/menu/JSON" - Retrieves all menu items of a restaurant
* "localhost:5000/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON" - Retrieves a specific menu item
