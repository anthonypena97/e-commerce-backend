# E-Commerce Backend
### A Backend for an E-Commerce Application
![MIT License badge](https://img.shields.io/badge/license-MIT_License-green)

![e-commerce-demo](https://user-images.githubusercontent.com/79285555/134746234-d9bea4ee-613b-44a1-967e-454205ec5400.gif)

<p> ---------------------------------------- </p>

Backend system written with [Node.js](https://nodejs.org/en/) using a [MySQL](https://www.mysql.com/) database.

The [Express](https://expressjs.com/), [MySql2](https://www.npmjs.com/package/mysql2), [Sequelize](https://www.npmjs.com/package/sequelize) and [dotenv](https://www.npmjs.com/package/dotenv) node packages are used.

## Description
The E-Commerce Back-End system established API calls for data base manipulation. With the integration of this Back-End system, an E-Commerce application will have the ability to transform and save Category, Product, and Tag data objects for the management of an merchant's inventory.

## Table of Contents
* [Installation](#installation)
* [Usage](#usage)
* [Routes](#routes)
* [License](#license)
* [Contributing](#contributing)
* [Testing](#testing)
* [Questions](#questions)
* [Acknowledgmenets](#Acknowledgments)

## Installation
*for this system to work, MySql and Node.js must be installed on your machine

- download or clone application
- open terminal in application root directory
- open ".env TEMPLATE", fill in with user_name and user_pass, rename to .env
- enter,`npm i`
- enter, `mysql -u { YOUR MYSQL USERNAME } -p`
- enter, `source ./db/schema.sql`
- enter,  `\quit`
- *for seeding data into database enter, `npm run seed`

- watch [video tutorial](https://drive.google.com/file/d/1MeD3rbZGGffwidG5Y7T2e2iXmYe6JIZU/view?usp=sharing) for in depth installation and usage

## Usage

```bash
npm start
```

## Routes

### Category
---
- GET Categories: .../api/categories
- GET Category: .../api/categories/:id
- POST Category: .../api/categories
```
{
	"category_name": "Sports Equipment" 
}
```
- PUT Category: .../api/categories/:id
```
{
	"category_name": "Sports Equipment" 
}
```
- DEL Category: .../api/categories/:id

### Product
---
- GET Products: .../api/proudcts
- GET Product: .../api/proudcts/:id
- POST Product: .../api/proudcts
```
{
	"product_name": "New York Yankees Hat",
  "price": 200.00,
  "stock": 3,
	"category_id": 4,
  "tagIds": [1, 2, 3, 4] 
}
```
- PUT Product: .../api/tags/:id
```
{
	"product_name": "Padrs Baseball Hat",
  "price": 200.00,
  "stock": 3,
	"category_id": 4,
  "tagIds": [1, 2, 3, 4] 
}
```
- DEL Product: .../api/tags/:id

### Tag
---
- GET Tags: .../api/tags
- GET Tag: .../api/tags/:id
- POST Tag: .../api/tags
```
{
	"tag_name": "New Wave"
}
```
- PUT Tag: .../api/tags/:id
```
{
	"tag_name": "Salsa"
}
```
- DEL Tag: .../api/tags/:id

## License
MIT License
    
Copyright (c) 2021 Anthony Pena

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation fil (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge,publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,subject to the following conditions:
            
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
            
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Version History
    
* 0.1
    * Initial Release
    * * See [commit change](https://github.com/anthonypena97/e-commerce-backend/commits/main) or See [release history](https://github.com/anthonypena97/e-commerce-backend/releases)

## Contributing
Please refer to the [Contributor Covenenant](https://www.contributor-covenant.org/) for guidelines on contributing on this project.

## Testing
API Routes may be tested on [Insomnia Core](https://insomnia.rest/products/insomnia)

## Questions
For any inquiries or questions, please contact Anthony Pena via:
* GitHub: [anthonypena97](https://github.com/anthonypena97)
* Email: <anthony.e.p3na@gmail.com>

## Acknowledgments

Inspiration, code snippets, etc.
* [Bootcamp Hotspot Starter Code](https://github.com/coding-boot-camp/fantastic-umbrella)
