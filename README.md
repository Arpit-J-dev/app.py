# app.py
REST API with Flask

Objective:
Create a REST API that manages user data using Python’s Flask framework.

Tools Required:
- Python
- Flask
- Postman or Curl (for testing)

Features:
The API supports the following HTTP methods:
- GET – Retrieve all users or a specific user by ID.
- POST – Add a new user.
- PUT – Update an existing user’s details.
- DELETE – Remove a user by ID.

Setup Instructions:
1. Install Flask:
   pip install flask
2. Save the provided Python code in a file named app.py
3. Run the application:
   python app.py
4. The API will be available at:
   http://127.0.0.1:5000

API Endpoints:

1. Get All Users
   Method: GET
   URL: /users
   Example Response:
   {
     "1": {"name": "John Doe", "email": "john@example.com"}
   }

2. Get a User by ID
   Method: GET
   URL: /users/<id>
   Example: /users/1

3. Add a New User
   Method: POST
   URL: /users
   Request Body (JSON):
   {
     "name": "John Doe",
     "email": "john@example.com"
   }

4. Update a User
   Method: PUT
   URL: /users/<id>
   Request Body (JSON):
   {
     "name": "Jane Doe"
   }

5. Delete a User
   Method: DELETE
   URL: /users/<id>

Example Curl Command:
curl -X POST -H "Content-Type: application/json" \
-d '{"name": "John Doe", "email": "john@example.com"}' \
http://127.0.0.1:5000/users

Outcome:
You will learn:
- Basics of REST API development with Flask
- Handling GET, POST, PUT, DELETE requests
- Testing APIs with Postman or Curl
