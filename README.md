#  Laravel with Docker Compose

A basic Laravel stack environment built using Docker Compose. It consists of the following:

* PHP
* Apache
* Postgress

As of now, we have several different PHP versions. Use appropriate php version as needed:

* 7.4.x
* 8.0.x

 
##  Installation
 
* Clone this repository on your local computer
* configure .env as needed 
* Run the `docker-compose up -d --build`.

## Set up the Laravel application

To set up the Laravel application, initiate a container in the php-apache container with the command below.

* `docker-compose exec php-apache /bin/bash`

* This opens a CLI in the php-apache container. Create the Laravel application using the following command.

* `composer create-project laravel/laravel .`

* Once this is completed, navigate to http://localhost/ which should display the default Laravel welcome page.

##  Configuration and Usage

### General Information 
This Docker Stack is build for local development and not for production usage.

### Configuration
This package comes with default configuration options. You can modify them by changing settings in `.env` file in your root directory.

### Configuration Variables
There are following configuration variables available and you can customize them by overwritting in your own `.env` file.

