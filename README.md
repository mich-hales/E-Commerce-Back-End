# E-Commerce Back End

## Description

This application is a backend service for an e-commerce site that involves the use of an express.js server and SQL database. It includes RESTful APIs which handle CRUD operations for organizing products, categories and tags. 


## Installation

* To get started, the user will need to naviagate to the cloned repository in their directory, and then run `npm install` to install `node.js`.

* Include the user's MYSQL user and password information in the .env file.

* To connect to the database, run the following commands:
  * `mysql -u root -p`
  * Type in the user's MYSQL password
  * `source db/schema.sql;`
  * `npm run seed`

* Run `npm start` to run the app and start the server. The user can then navigate to the port displayed in the terminal or use Insomnia.

## Usage

* When the user adds the database name, MySQL username, and MySQL password to an environment variable file, then they will be able to connect to a database using Sequelize.
* When the user enters schema and seed commands, a development database is created and is seeded with test data.
* When the user enters the command to invoke the application, then the server is started and the Sequelize models are synced to the MySQL database.
* When the user opens API GET routes in Insomnia for categories, products, or tags, the data for each of these routes is displayed in a formatted JSON.
* When the user tests API POST, PUT, and DELETE routes in Insomnia, they are able to successfully create, update, and delete data in their database.

## Mock-Up

The following video shows how to start the application along with the application being tested in Insomnia:

https://user-images.githubusercontent.com/107455470/196297882-e9a2e854-d1fa-441e-af43-61661d7000e3.mp4

GitHub Repository: https://github.com/mich-hales/E-Commerce-Back-End