# 📘 Assignment: Testing FastAPI Applications with pytest

## 🎯 Objective

Write automated tests for the book catalog API from the FastAPI assignment. Use pytest and FastAPI's TestClient to check successful requests, request validation, and error responses without starting a web server.

## 📝 Tasks

### 🛠️ Test Successful API Requests

#### Description
Create a pytest test suite for the book catalog endpoints. Use TestClient to send requests and verify that the API returns the expected status codes and JSON data.

#### Requirements
Completed program should:

- Use pytest and FastAPI's `TestClient`
- Test that `GET /books` returns a successful response with a JSON list
- Test that `POST /books` creates a book and returns its expected fields
- Test retrieving, updating, and deleting a book by ID
- Verify that the book is updated and no longer available after deletion


### 🛠️ Test Validation and Error Responses

#### Description
Add tests for invalid requests and IDs that do not match an existing book. Make sure each test starts from a predictable state so results do not depend on test order.

#### Requirements
Completed program should:

- Test that requesting a book with an unknown ID returns HTTP `404`
- Test that a request with missing or invalid book fields returns HTTP `422`
- Reset or isolate the in-memory book data between tests
- Run the full test suite with pytest and confirm all tests pass
