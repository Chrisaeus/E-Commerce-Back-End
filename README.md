# E-Commerce Back End

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://www.contributor-covenant.org/version/2/1/code_of_conduct/)

## Description

This app simulates the functionality of an E-Commerce Back End, allowing the user to populate a MySQL database with products with custom categories and tags. The app comes with a seed for populating the database with example products, categories, and tags. Routes are set up to allow products, categories, and tags to be created and deleted as well as modified through HTTP requests.

The E-Commerce Back End uses MySQL2 and uses Sequelize to connect the database to an Express server. A dotenv file needs to be created to store the database credentials.


---

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Contributing](#contributing)
4. [Tests](#tests)
5. [License](#license)
6. [Questions](#questions)

---

## Installation

1. This application requires Node.js. Download it at <https://nodejs.org>.

2. Open command line to repository root directory. Enter `npm i` to download the dependencies.

3. Use the `schema.sql` file in the `db` directory to create the database using your MySQL shell.

4. Create a .env file in the root directory and enter your MySQL credentials. Formatting:

    `DB_USER=''`

    `DB_PW=''`

    `DB_NAME='ecommerce_db'`

5. To populate the database with example data, run `npm run seed`.

6. Start the app server with `npm start`.


---

## Usage

Use a program like Insomnia to send HTTP requests to the server once it's running.

The endpoints are as follows:

1. `http://localhost:3001/products`

2. `http://localhost:3001/categories`

3. `http://localhost:3001/tags`

Sending GET or POST requests to these endpoints will respectively retrieve all data points in the corresponding table or create a new data point. The endpoints are set up to recieve JSON request bodies.

Appending the ID number of a product, category, or tag to the end of the appropriate endpoint allows for updating data with PUT requests or deleting data with DELETE requests.

<br />

#### Here's a gif showing some of the functionality using Insomnia - click to open the full video:

[![Insomnia Example](<./assets/images/E-Commerce Back End.gif>)](https://watch.screencastify.com/v/81lEARjtbNUS2geVNSwd)


---

## Contributing

Any contributions that conform to the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/) are welcome!


---

## Tests

There are no built-in tests included in this application, but a program like Insomnia that simulates HTTP requests can be used to test the functionality of the app.


---

## License

MIT License

Copyright &copy; 2022 Christian Sadler

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

## Questions

If you have questions, contact me on [GitHub](https://github.com/Chrisaeus) or send me an e-mail at <christian.sadler@yahoo.com>.