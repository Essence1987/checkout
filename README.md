# **E-commerce Application** [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is an e-commerce application that provides a backend server for managing products, categories, and tags. It leverages Sequelize as the ORM (Object-Relational Mapping) to interact with a MySQL database.

#**Table of Contents**<br><ul><li>[Features](#features)</li><li>[Installation](#installation)</li><li>[Usage](#usage)</li><li>[Technology](#technology)</li><li>[Database Schema](#database-schema)</li><li>[Tests](#tests)</li><li>[Credits](#credits)</li><li>[Contribute](#contribute)</li><li>[Questions](#questions)</li><li>[License](#license)</li></ul>

## **Features**

- View all products, categories, and tags: Display lists of products, categories, and tags stored in the database.
- Add new products, categories, and tags: Add new items to the database.
- Update product details: Modify product information such as name, price, or availability.
- Associate products with categories and tags: Categorize products and add tags to facilitate searching.
- Delete products, categories, and tags: Remove items from the database.
</br></br>

## **Installation**

1. Clone the repository to your local machine using the following command in your terminal: git@github.com:Essence1987/tracker.git
2. If needed, install the required dependencies by running the following command in the project directory: npm install
3. Rename .env.EXAMPLE to .env and update the Username and Password to match your MySql database credentials.
4. Set up your MySQL database by importing the schema.sql file provided in the repository db folder.
5. Exit MySql and Seed the demo content for the tables by running node seeds/index.js
6. Start the application by running the following command: node server.js</br></br>

## **Usage**

The backend server will now be running, allowing you to perform various CRUD (Create, Read, Update, Delete) operations through API endpoints. You can use tools like Insomnia or integrate the API with a front-end application to interact with the e-commerce database.

For a demonstration, please watch the following video:

The first video shows GET routes to return all categories, all products, and all tags being tested in insomnia:

The second video shows GET routes to return a single category, a single product, and a single tag being tested in Insomnia:

The third video shows the POST, PUT, and Delete routes for catagories being tested in Insomnia.



## **Technology**

* Node.js
* MySQL
* Sequelize (ORM)
* Express.js (Web framework)
* Dotenv (Environment Variables)

## **Database Schema**

The database schema for this project includes the following tables:

### Categories table:

* id (INT, Primary Key, Auto Increment)
* category_name (VARCHAR(100))

### Products table:

* id (INT, Primary Key, Auto Increment)
* product_name (VARCHAR(255))
* price (DECIMAL(10, 2))
* stock (INT)
* category_id (INT, Foreign Key referencing categories.id)

### Tags table:

* id (INT, Primary Key, Auto Increment)
* tag_name (VARCHAR(100))

### ProductTags table:

* id (INT, Primary Key, Auto Increment)
* product_id (INT, Foreign Key referencing products.id)
* tag_id (INT, Foreign Key referencing tags.id)
</br></br>

## **Test**

No tests are currently implemented for this project.

## **Credits**

This was a solo project with no contributers taking part.

## **Contribute**

This is a personal project, and contributions are not accepted at this time.

## **Questions**

Click the image below to go to my github page!

<a href="https://github.com/essence1987"><img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=essence1987&theme=default"/></a>

If you have any questions or need further assistance, please feel free to contact me:

My email is hwmelander@gmail.com

## **License**

Employee Tracking Database is released under [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT). Click on the badge for more information.
