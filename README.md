
# Library API

## Overview

The Library API is a backend service designed to manage library resources such as books, authors, and user records. Built using the Slim PHP micro-framework, this API provides efficient and scalable solutions for library management, including authentication and resource handling.

## Features

- **RESTful API Endpoints** for managing library operations.
- **Authentication** using JSON Web Tokens (JWT).
- Lightweight and scalable, leveraging the Slim PHP framework.
- Easy integration with relational databases (schema included in `library.sql`).

## Installation

### Prerequisites

- PHP 7.4 or later
- Composer (PHP Dependency Manager)
- A web server (e.g., Apache or Nginx)
- A MySQL database

### Steps

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Navigate to the `src` directory:
   ```bash
   cd src
   ```

3. Install dependencies using Composer:
   ```bash
   composer install
   ```

4. Import the database schema:
   - Locate the `library.sql` file in the root directory.
   - Import it into your MySQL database:
     ```bash
     mysql -u <username> -p <database_name> < library.sql
     ```

5. Configure the database connection:
   - Update the configuration file (if present) with your database credentials.

6. Start the server:
   - Use PHP's built-in server for local testing:
     ```bash
     php -S localhost:8000 -t public
     ```
   - Alternatively, configure a virtual host on your web server.

## Usage

Access the API via `http://localhost:8000` (or your configured domain). Use tools like Postman or curl to test the endpoints.

### Authentication

Use the JWT library for generating and validating tokens. Authentication endpoints require a valid token.

## Endpoints

Commonly implemented endpoints include:

- **Books**
  - `GET /books`: Fetch all books.
  - `POST /books`: Add a new book.

- **Authors**
  - `GET /authors`: Fetch all authors.
  - `POST /authors`: Add a new author.

- **Authentication**
  - `POST /login`: Authenticate a user and obtain a JWT.

(Note: The actual endpoints may vary based on the implementation. Refer to the source code for detailed routing.)

## Database

The `library.sql` file contains the schema required to set up the database. Ensure that the database is properly configured before using the API.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Description of changes"`.
4. Push to the branch: `git push origin feature-name`.
5. Create a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for more information.

---

Happy coding! 🎉
if  you need more information about this, don't hesitate to contact me on my email "hcarig80@gmail.com" and on facebook "Hannah Grace" THANK YOUUUU <3
