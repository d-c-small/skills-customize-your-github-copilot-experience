# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Students will learn to create RESTful APIs using the FastAPI framework in Python, including defining endpoints, handling HTTP requests, and returning JSON responses.

## 📝 Tasks

### 🛠️ Set Up FastAPI and Basic Endpoint

#### Description
Install FastAPI and create a simple API that returns a "Hello World" message at the root endpoint.

#### Requirements
Completed program should:

- Install FastAPI and uvicorn using pip
- Create an endpoint at `/` that returns `{"message": "Hello World"}`
- Run the server with `uvicorn main:app --reload` and verify the endpoint works

### 🛠️ Implement CRUD Operations

#### Description
Add endpoints to perform Create, Read, Update, and Delete operations on a list of items.

#### Requirements
Completed program should:

- Include a POST endpoint at `/items` to create a new item
- Include a GET endpoint at `/items` to retrieve all items
- Include a GET endpoint at `/items/{item_id}` to retrieve a specific item by ID
- Include a PUT endpoint at `/items/{item_id}` to update an existing item
- Include a DELETE endpoint at `/items/{item_id}` to delete an item
- Use an in-memory list to store items (e.g., list of dictionaries with id, name, description)

### 🛠️ Add Validation and Documentation

#### Description
Use Pydantic models for request and response validation, and ensure the API generates automatic documentation.

#### Requirements
Completed program should:

- Define Pydantic BaseModel classes for Item creation and response
- Validate incoming request data using the models
- Access the interactive API documentation at `/docs`
- Ensure all endpoints handle validation errors appropriately