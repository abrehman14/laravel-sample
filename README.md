<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## Image Temporary Url Generation
Its a sample code in which we store a user with  params name,type,description and file. The file is basically an
image **maxsize of 5MB**   which is stored in the private directory and we generate the temporary url for the file which
will  expire after 10 mints, And has a cron job implemented which will run every hour and will remove the 30 days old record.

###  Concepts Implemented
- Single Responsibility Principle
- Code Abstraction Using Interfaces and Services
- Data Transfer Object
- Request Validations
- Docker
- Test Driven Apis
- Code Coverage
- Code Coverage Reports Generation
 
###  Third Party Package Used

- [Intervention / image](https://github.com/Intervention/image)

## Project Setup
This project has both the support to run either on the docker or you can also run it as a simple laravel project

## Laravel Run Environment Dependence

- PHP 8.1
- Composer
- Mysql
- Xdebug Extension

#### Setup 
- Create the Database.
- Copy the .env.example to .env
- Change the Database Environment Variables Values
- Run the command **composer install**
- Run the command **php artisan migrate && php artisan serve**


## Docker Environment
- Docker Engine

#### Setup
- Copy the .env.example to .env
- Change the Database Environment Variables Values
- Just run the command **docker compose up**
- Then go in the backend container 
- Run the command **php artisan migrate** 

## Tests & Code Coverage
- This project has implemented the unit test which you can run using command **php artisan test**
- To see the code coverage you can run the command **XDEBUG_MODE=coverage php artisan test --coverage**
- To Generate the code coverage reports run the command **XDEBUG_MODE=coverage vendor/bin/phpunit --coverage-html reports**
- You can also view the coverage reports by opening index.html file under the folder **reports**


<br/><br/><br/>