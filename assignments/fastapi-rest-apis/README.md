# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a REST API with FastAPI to practice defining endpoints, handling JSON data, validating requests, and using HTTP methods and status codes. You will create an in-memory book catalog that supports the basic CRUD operations.

## 📝 Tasks

### 🛠️ Create the Book API

#### Description
Create a FastAPI application for a book catalog. Define a book data model and implement endpoints to list all books and add a new book.

#### Requirements
Completed program should:

- Define a Pydantic model with a book title and author
- Implement `GET /books` to return the catalog as JSON
- Implement `POST /books` to add a book from a JSON request body
- Keep the catalog in memory; a database is not required


### 🛠️ Add Book Management Endpoints

#### Description
Extend the API so clients can retrieve, update, and delete an individual book by its ID.

#### Requirements
Completed program should:

- Assign each book a unique ID
- Implement `GET /books/{book_id}` to return one book
- Implement `PUT /books/{book_id}` to update a book's title and author
- Implement `DELETE /books/{book_id}` to remove a book
- Return an appropriate not-found response when a requested book ID does not exist
