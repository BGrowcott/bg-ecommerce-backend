# E-Commerce Backend

## Description

This project represents the backend for an e-commerce back end. This uses Express.js API and Sequelize to interact with a MySQL database. Calls to the API allows a user to Create, Read, Update and Delete from the database.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Video Demonstration](#demo-video)
4. [Contributing](#contributing)
6. [Questions](#questions)

## Installation
----
1. Git clone this repository
2. Navigate to the correct directory in your command line
3. Add database name, mySQL username and mySQL to an environment variable file
3. Open mySQL command line and source the database schema
4. Exit mySQL and run command: node seeds/index.js
3. Run command: npm install
4. Run command: npm start
5. Use Postman/Insomnia to check the api calls
----

## Usage

- Once a user has followed the installation instructions they can connect to the database using Sequelize.
  - Entering the schema and seed commands created the database and seeds it with test data.
  - Starting the application syncs Sequelize models to the database.

- Running GET routes in Postman/Insomnia the data for each route is displayed in formatted JSON.
  - Running POST, PUT and DELETE routes allows a user to create, update and delete data in the database.

### Route examples:

#### Categories

Get all:
```
GET localhost:3001/api/categories
```
Get single:
```
GET localhost:3001/api/categories/{{id}}
```
Create new:
```
POST localhost:3001/api/categories
Body: category_name: {{name here}}
```
Update:
```
PUT localhost:3001/api/categories/{{id}}
Body: category_name: {{updated name}}
```
Delete:
```
DELETE localhost:3001/api/categories/{{id}}
```

#### Tags

Get all:
```
GET localhost:3001/api/tags
```
Get a single:
```
GET localhost:3001/api/tags/{{id}}
```
Create new:
```
POST localhost:3001/api/tags
Body: tag_name: {{name here}}
```
Update:
```
PUT localhost:3001/api/tags/{{id}}
Body: tag_name: {{updated name}}
```
Delete:
```
DELETE localhost:3001/api/tags/{{id}}
```

#### Products

Get all:
```
GET localhost:3001/api/products
```
Get a single:
```
GET localhost:3001/api/products/{{id}}
```
Create new:
```
POST localhost:3001/api/products
example Body:     
    {
      product_name: "Basketball",
      price: 200.00,
      stock: 3,
      tagIds: [1, 2, 3, 4]
    }
```
Update:
```
PUT localhost:3001/api/products/{{id}}
example Body:     
    {
      price: 150.00,
      stock: 1,
    }
```
Delete:
```
DELETE localhost:3001/api/products/{{id}}
```

### Demo video

Please check out this video of the application in action - [Video](https://drive.google.com/file/d/1cV8IAg-KsX0nl9M9XZJ9g10SwnZXDsFs/view?usp=sharing)

## Contributing

Ben Growcott - [GitHub](https://github.com/BGrowcott)

## Questions

If you have any questions or suggestions please contact me via my GitHub or Email:

[GitHub](https://github.com/BGrowcott)

[Email](mailto:bg.coding101@gmail.com)

----