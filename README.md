# 13-ORM-ecommerce-backend

## Description
Using express.js and Sequelize to communicate with a MySQL database, I was able to create a back-end application for an e-commerce website. I tested my GET, PUT, POST and DELETE routes in Insomnia to ensure all back-end routes were functional. 

## Table of Contents
* [User Story](#user-story)
* [Acceptance Criteria](#acceptance-criteria)
* [Installation](#installation)
* [Usage](#usage)
* [Sources](#sources)
* [Issues](#issues)
* [Link to Recordings](#link-to-recordings)

## User Story
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

## Acceptance Criteria
- GIVEN a functional Express.js API
- WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
- THEN I am able to connect to a database using Sequelize
- WHEN I enter schema and seed commands
- THEN a development database is created and is seeded with test data
- WHEN I enter the command to invoke the application
- THEN my server is started and the Sequelize models are synced to the MySQL database
- WHEN I open API GET routes in Insomnia Core for categories, products, or tags
- THEN the data for each of these routes is displayed in a formatted JSON
- WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
- THEN I am able to successfully create, update, and delete data in my database

## Installation
* Begin by opening an Integrated terminal in VS Code and runnning command 'npm i' to install all necessary dependencies for this application.
* Naviagte to your 'schema.sql' and open a new Integrated terminal and run command 'mysql -u root -p' 
* Enter your MySQL password
* Then run command 'source schema.sql' to create database.
* Next run command 'node seeds/index.js' in root directory terminal
* Finally run command 'node server.js' to initialize the server.
* If done correctly you will recieve 'App listening on port 3001' message to confirm server has been started.

## Sources
* [Express.js Documentation](https://expressjs.com/)
* [MySQL Documentation](https://dev.mysql.com/doc/)
* [Sequelize Documentation](https://sequelize.org/master/)
* [dotenv Documentation](https://www.npmjs.com/package/dotenv)
* [Insomnia Documentation](https://support.insomnia.rest/)
* [W3Schools](https://www.w3schools.com/)
* [npm Documentation](https://docs.npmjs.com/)

## Issues
- I ran into issues within my database, I kept recieving errors about duplicate columns being created and was able to correct those issues, which ended up being minor syntax errors
- This took up a lot of my time combing through my code to find the bugs, so I was not able to complete testing my PUT and DELETE routes. 
- On that note I was able to nail down GET routes for 'Products' and 'Category', but recieved an erorr when testing GET routes for 'Tag'
- I think this is an issue with seeding my database tables correctly but did not have enough time to fix the bugs

## Link to Recording

[Link to vide demo](https://drive.google.com/file/d/1nojoMi-MvtBSk8EYDWQnPy3ylz-c5mZc/view)

