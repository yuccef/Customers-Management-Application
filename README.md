# Introduction

Welcome to the Customers Management Application! This web application is designed to help you manage your customers in an easy and efficient way. With this application, you can view, add, modify, and delete customer information all in one place.


# Getting started

 ## Installation

To install the project, you need to clone the repository from Github or Gitlab.


git clone https://github.com/yuccef/Customers-management-Application.git

Next, navigate to the project directory and install the dependencies using npm:

      cd Customers-management-Application
      npm install


## Usage

To start the web server, you need to run the following command.

      npm start

 The web server will start listening on port 3001. You can access the application by visiting http://localhost:3001.

# Functionnalities

## Displaying the Data (JSON)

To display the Data of customers, you can access the following URL: http://localhost:3001/api/customers. It will return a JSON array of all the customers.


To display the Data of a specefic customer, you can access the following URL: http://localhost:3001/api/customers/id/:id. It will return a JSON array of the customer.

## Displaying the list of customers

To display the list of customers, you can access the following URL: http://localhost:3001/api/customers/liste. It will return a HTML page of all the customers with pagination.


## Adding a new customer

To add a new customer, you can access the following URL: http://localhost:3001/api/customers/add. You will need to submit a POST request with the following parameters:

    email (string, required): the email address of the customer
    first (string, required): the first name of the customer
    last (string, required): the last name of the customer
    company (string, required): the name of the company of the customer
    country (string, required): the country of the customer

The server will generate an id and a creation date automatically.

HTML page for Adding a customer is http://localhost:3001/api/customers/liste/add.


## Modifying a customer

To modify an existing customer, you can access the following URL: http://localhost:3001/api/customers/id/:id, where :id is the id of the customer you want to modify. You will need to submit a PUT request with the following parameters:

    email (string, required): the email address of the customer
    first (string, required): the first name of the customer
    last (string, required): the last name of the customer
    company (string, required): the name of the company of the customer
    country (string, required): the country of the customer

HTML page for Modifying a customer is http://localhost:3001/api/customers/liste/modify.

## Deleting a customer

To Delete an existing customer, you can access the following URL: http://localhost:3001/api/customers/delete. You will need to submit a DELETE request with the following parameters:

    Id  (id, required): the Id of the customer
 
HTML page for Deleting a customer is http://localhost:3001/api/customers/liste/delete.



# Development

## Project structure

The project is structured as follows:

    index.js: the entry point of the application
    Server/data/customers.json: the JSON file containing the list of customers

To start the Application, run:
     npm start


## Coding style

 The project follows JavaScript style guide. ESLint is used to enforce this style guide. You can run ESLint by running the following command:

    npm run lint


 ## Test 
 
In addition to the main functionalities provided by the web application, you can also test some operations directly on the database without the need for a server.

Simply navigate to the "server" folder and run the "backTestForConsole.js" file. This will allow you to interact with the database through the console. This can be a useful tool for testing and debugging your application.

So, if you want to experiment and test the database operations without running the entire application, the "backTestForConsole.js" file is a great option.


# Conclusion

This project provides powerful functionality to manage a list of customers. With a user-friendly interface and efficient data management, the Customers Management Application is an ideal solution for businesses of all sizes.