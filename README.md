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

The following animation shows the application's GET routes to return all categories, all products, and all tags being tested in Insomnia:

![In Insomnia, the user tests “GET tags,” “GET Categories,” and “GET All Products.”.](./Assets/13-orm-homework-demo-01.gif)

The following animation shows the application's GET routes to return a single category, a single product, and a single tag being tested in Insomnia:

![In Insomnia, the user tests “GET tag by id,” “GET Category by ID,” and “GET One Product.”](./Assets/13-orm-homework-demo-02.gif)

The following animation shows the application's POST, PUT, and DELETE routes for categories being tested in Insomnia:

![In Insomnia, the user tests “DELETE Category by ID,” “CREATE Category,” and “UPDATE Category.”](./Assets/13-orm-homework-demo-03.gif)

Your walkthrough video should also show the POST, PUT, and DELETE routes for products and tags being tested in Insomnia.

### Sync Sequelize to the Database on Server Start

Create the code needed in `server.js` to sync the Sequelize models to the MySQL database on server start.


### Walkthrough Video: 37%

* A walkthrough video that demonstrates the functionality of the e-commerce back end must be submitted, and a link to the video should be included in your readme file.

* The walkthrough video must show all of the technical acceptance criteria being met.

* The walkthrough video must demonstrate how to create the schema from the MySQL shell.

* The walkthrough video must demonstrate how to seed the database from the command line.

* The walkthrough video must demonstrate how to start the application’s server.

* The walkthrough video must demonstrate GET routes for all categories, all products, and all tags being tested in Insomnia.

* The walkthrough video must demonstrate GET routes for a single category, a single product, and a single tag being tested in Insomnia.

* The walkthrough video must demonstrate POST, PUT, and DELETE routes for categories, products, and tags being tested in Insomnia.

### Technical Acceptance Criteria: 40%

* Satisfies all of the preceding acceptance criteria plus the following:

  * Connects to a MySQL database using the [MySQL2](https://www.npmjs.com/package/mysql) and [Sequelize](https://www.npmjs.com/package/sequelize) packages.

  * Stores sensitive data, like a user’s MySQL username, password, and database name, using environment variables through the [dotenv](https://www.npmjs.com/package/dotenv) package.

  * Syncs Sequelize models to a MySQL database on the server start.

  * Includes column definitions for all four models outlined in the Challenge instructions.

  * Includes model associations outlined in the Challenge instructions.

## Review

You are required to submit BOTH of the following for review:

* A walkthrough video demonstrating the functionality of the application and all of the acceptance criteria being met.

* The URL of the GitHub repository. Give the repository a unique name and include a readme describing the project.
