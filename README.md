# Library-Spring-Rest-API-Project

This is a Spring Boot application for managing a library system. The application provides CRUD operations for managing books, authors, book borrowings, categories, and publishers.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/library-application.git
    ```
2. Navigate to the project directory:
    ```bash
    cd library-application
    ```
3. Build the project with Maven:
    ```bash
    mvn clean install
    ```
4. Run the application:
    ```bash
    mvn spring-boot:run
    ```

## Usage

The application will be running at `http://localhost:8080`. You can interact with the API using tools like Postman or Curl.

## API Endpoints

### Books

| Method | Endpoint           | Description                 | Request Body           | Response       |
|--------|--------------------|-----------------------------|------------------------|----------------|
| GET    | `/v1/books`        | Get all books               | N/A                    | 200 OK         |
| GET    | `/v1/books/{id}`   | Get a book by ID            | N/A                    | 200 OK         |
| POST   | `/v1/books`        | Add a new book              | JSON representation of the book | 201 Created   |
| PUT    | `/v1/books/{id}`   | Update a book               | JSON representation of the updated book | 200 OK    |
| DELETE | `/v1/books/{id}`   | Delete a book               | N/A                    | 204 No Content |

### Authors

| Method | Endpoint           | Description                 | Request Body           | Response       |
|--------|--------------------|-----------------------------|------------------------|----------------|
| GET    | `/v1/authors`      | Get all authors             | N/A                    | 200 OK         |
| GET    | `/v1/authors/{id}` | Get an author by ID         | N/A                    | 200 OK         |
| POST   | `/v1/authors`      | Add a new author            | JSON representation of the author | 201 Created   |
| PUT    | `/v1/authors/{id}` | Update an author            | JSON representation of the updated author | 200 OK    |
| DELETE | `/v1/authors/{id}` | Delete an author            | N/A                    | 204 No Content |

### Book Borrowings

| Method | Endpoint                 | Description                 | Request Body           | Response       |
|--------|--------------------------|-----------------------------|------------------------|----------------|
| GET    | `/v1/bookborrowings`     | Get all book borrowings     | N/A                    | 200 OK         |
| GET    | `/v1/bookborrowings/{id}`| Get a book borrowing by ID  | N/A                    | 200 OK         |
| POST   | `/v1/bookborrowings`     | Add a new book borrowing    | JSON representation of the book borrowing | 201 Created   |
| PUT    | `/v1/bookborrowings/{id}`| Update a book borrowing     | JSON representation of the updated book borrowing | 200 OK    |
| DELETE | `/v1/bookborrowings/{id}`| Delete a book borrowing     | N/A                    | 204 No Content |

### Categories

| Method | Endpoint           | Description                 | Request Body           | Response       |
|--------|--------------------|-----------------------------|------------------------|----------------|
| GET    | `/v1/categories`   | Get all categories          | N/A                    | 200 OK         |
| GET    | `/v1/categories/{id}` | Get a category by ID    | N/A                    | 200 OK         |
| POST   | `/v1/categories`   | Add a new category          | JSON representation of the category | 201 Created   |
| PUT    | `/v1/categories/{id}` | Update a category       | JSON representation of the updated category | 200 OK    |
| DELETE | `/v1/categories/{id}` | Delete a category       | N/A                    | 204 No Content |

### Publishers

| Method | Endpoint           | Description                 | Request Body           | Response       |
|--------|--------------------|-----------------------------|------------------------|----------------|
| GET    | `/v1/publishers`   | Get all publishers          | N/A                    | 200 OK         |
| GET    | `/v1/publishers/{id}` | Get a publisher by ID    | N/A                    | 200 OK         |
| POST   | `/v1/publishers`   | Add a new publisher         | JSON representation of the publisher | 201 Created   |
| PUT    | `/v1/publishers/{id}` | Update a publisher       | JSON representation of the updated publisher | 200 OK    |
| DELETE | `/v1/publishers/{id}` | Delete a publisher       | N/A                    | 204 No Content |

## Contributing

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes.
4. Commit your changes:
    ```bash
    git commit -m "Add new feature"
    ```
5. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
6. Open a pull request.

