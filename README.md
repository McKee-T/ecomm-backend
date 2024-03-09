# E-Commerce Backend

## Description

This project provides a backend for an e-commerce site, leveraging Express.js for the server and Sequelize as the ORM to interact with a MySQL database. It supports CRUD operations for products, categories, and tags, making it a versatile backend solution for e-commerce applications.

## Features

- RESTful API for managing e-commerce data.
- Models for Products, Categories, and Tags with associations.
- Sequelize for database schema creation, seeding, and query handling.
- Environment configuration for database connection details.

## Installation

1. Clone the repository to your local machine.
   ```
   git clone https://github.com/McKee-T/ecomm-backend.git
   ```
2. Navigate to the project directory.
   ```
   cd ecomm-backend
   ```
3. Install the necessary dependencies.
   ```
   npm install
   ```
4. Create a `.env` file in the root directory with the following content, replacing values as per your MySQL setup:
   ```
   DB_NAME='ecommerce_db'
   DB_USER='your_mysql_username'
   DB_PASSWORD='your_mysql_password'
   ```

## Database Setup

1. Log in to your MySQL shell and create the database:
   ```sql
   CREATE DATABASE ecommerce_db;
   ```
2. Exit the MySQL shell and run the Sequelize migrations to create the tables and seed the data:
   ```
    node seeds/index.js
   ```

## Usage

1. Start the server:
   ```
   npm start
   ```
2. Use a tool like Postman or Insomnia to test the API endpoints. The base URL is `http://localhost:3001/api`.

### Endpoints

- **Products**: `/api/products` (GET, POST), `/api/products/:id` (GET, PUT, DELETE)
- **Categories**: `/api/categories` (GET, POST), `/api/categories/:id` (GET, PUT, DELETE)
- **Tags**: `/api/tags` (GET, POST), `/api/tags/:id` (GET, PUT, DELETE)

## Testing

Ensure you have Postman or Insomnia installed to test the API endpoints. Import the provided collection (if available) or manually set up requests to test each endpoint.

## Contribution

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Commit your changes with a clear description.
4. Push your branch and open a pull request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Questions

If you have any questions or encounter issues, please open an issue on the GitHub repository or contact the project owner.
