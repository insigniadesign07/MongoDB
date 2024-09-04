# Node.js MongoDB CRUD API
This repository contains a Node.js application with MongoDB integration for performing CRUD operations on user data. The application uses Express.js for the server and Mongoose for MongoDB interaction.

# Installation
Clone the Repository:

# bash
Copy code
git clone https://github.com/yourusername/node-mongo-crud.git
Navigate to Project Directory:

# bash
Copy code
cd node-mongo-crud
Install Dependencies:

# bash
Copy code
npm install
Create a .env File:

Create a .env file in the root directory with the following content:

# env
Copy code
MONGO_URI=mongodb://localhost:27017/yourdb
Run the Application:

# bash
Copy code
npm start
The server will start on http://localhost:3000.

API Endpoints
Retrieve All Users

Method: GET
URL: http://localhost:3000/api/users
Retrieve a Specific User by ID

# Method: GET
URL: http://localhost:3000/api/users/:id
Example URL: http://localhost:3000/api/users/1
Create a New User

# Method: POST

URL: http://localhost:3000/api/users

Request Body:

# json
Copy code
{
  "name": "Ahmad",
  "email": "ahmad@gmail.com"
}
Update an Existing User

# Method: PUT

URL: http://localhost:3000/api/users/:id

Example URL: http://localhost:3000/api/users/1

Request Body:

# json
Copy code
{
  "name": "Raza",
  "email": "razaraza@gmail.com"
}
# Delete a User

# Method: DELETE
URL: http://localhost:3000/api/users/:id
Example URL: http://localhost:3000/api/users/1
Testing with Postman
Open Postman and create a new request.

Set Up Your Requests:

Retrieve All Users

# Method: GET
URL: http://localhost:3000/api/users
Retrieve Specific User

# Method: GET
URL: http://localhost:3000/api/users/{id}
Create User

# Method: POST

URL: http://localhost:3000/api/users

Body:

json
Copy code
{
  "name": "Ahmad",
  "email": "ahmad@gmail.com"
}
Update User

Method: PUT

URL: http://localhost:3000/api/users/{id}

Body:

json
Copy code
{
  "name": "raza",
  "email": "razaraza@gmail.com"
}
Delete User

# Method: DELETE
URL: http://localhost:3000/api/users/{id}
Send Requests and check the responses to ensure your API is functioning correctly.

Contributing
Feel free to contribute by submitting issues or pull requests. Please follow the project's coding style and guidelines.

