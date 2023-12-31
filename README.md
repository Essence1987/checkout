# **E-commerce Application** [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is an e-commerce application that provides a backend server for managing products, categories, and tags. It leverages Sequelize as the ORM (Object-Relational Mapping) to interact with a MySQL database.

#**Table of Contents**<br><ul><li>[Features](#features)</li><li>[Installation](#installation)</li><li>[Usage](#usage)</li><li>[Technology](#technology)</li><li>[Database Schema](#database-schema)</li><li>[Tests](#tests)</li><li>[Credits](#credits)</li><li>[Contribute](#contribute)</li><li>[Questions](#questions)</li><li>[License](#license)</li></ul>

## **Features**

- View all products, categories, and tags: Display lists of products, categories, and tags stored in the database.
- Add new products, categories, and tags: Add new items to the database.
- Update product details: Modify product information such as name, price, or availability.
- Associate products with categories and tags: Categorize and add tags to facilitate searching.
- Delete products, categories, and tags: Remove items from the database.
</br></br>

## **Installation**

1. Clone the repository to your local machine using the following command in your terminal: git@github.com:Essence1987/tracker.git
2. Open your terminal and ensure you are pointed at the public folder.
3. If needed, install the required dependencies by running the following command in the project directory: npm install
4. Rename .env.EXAMPLE to .env and update the Username and Password to match your MySql database credentials.
5. Set up your MySQL database by importing the schema.sql file in the repository db folder.
6. Exit MySql and Seed the demo content for the tables by running node seeds/index.js
7. Start the application by running the following command: node server.js</br></br>

For a demonstration of installation, please watch the following video, which starts from step 4:

https://github.com/Essence1987/checkout/assets/129245370/c11030f3-788d-4fed-95a4-6e70d89452d1



## **Usage**

The backend server will run, allowing you to perform various CRUD (Create, Read, Update, Delete) operations through API endpoints. You can use tools like Insomnia or integrate the API with a front-end application to interact with the e-commerce database.

For a demonstration, please watch the following videos:

The first video shows GET routes to return all categories, all products, and all tags being tested in insomnia:


https://github.com/Essence1987/checkout/assets/129245370/d7f8357d-9e0e-45c6-bd9b-cfc606f30e2d


The second video shows GET routes to return a single category, a single product, and a single tag being tested in Insomnia:


https://github.com/Essence1987/checkout/assets/129245370/aa222343-ce2c-4013-abe6-410a3df4be1b


The third video shows the POST, PUT, and Delete routes for categories being tested in Insomnia.


https://github.com/Essence1987/checkout/assets/129245370/c95c7c62-a01d-4b90-b237-151ae3545647




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
