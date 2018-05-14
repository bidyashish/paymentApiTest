This is a simple LARAVEL Application based on  LARAVEL 5.5 LTS   for API Authentication.

Solution for Test https://github.com/claytonchew/developer-assessment-tests/tree/master/backend/intermediate_lead/part2

Usage :
Create a registration API that requires the user to send in their username, password, and their account type for registration. Each user gets RM 100 upon registration.
Create a login API that logs the user into the system.
Create an API that allows a user to send money to another user.


Project info:

This project has sqlite DB in database folder


Installation:

1. Download the Project as Zip or fork it.

2. Open .env file set the database prim.sqlite file path
   In Linux Environment use   pwd in folder and set the path
   In Windows get folder address and set the file path for prim.sqlite

3. In PHP( 7.1+ only) Dev Environment  Run Command  
   Note  : Must have ALL PHP and SQLITE SETUP
    
      php artisan serve
5.  Project has three ENDPOINT /login  ,  /register   , /transfer

4.   Open postman set POST request  and  Body as  raw and header type JSON

    URL   http://localhost:8000/api/register

      JSON  to send   :     {   "name": "Ashish", "email": "bidya@bidya.com", "type" : "customer","password": "mypass","c_password" :"mypass"  }
                  
                 
    http://localhost:8000/api/login

     JOSN to login :  { 	"email":"bisssssdya@bidssya.com", "password":"mypass" }  

5. http://localhost:8000/api/transfer

