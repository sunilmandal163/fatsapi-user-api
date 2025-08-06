FastAPI User Management API:
This is a simple user management API built with FastAPI and PostgreSQL. The goal of this project was to learn how to create a RESTful API using modern Python tools and best practices, including async database access with SQLAlchemy.

What this project does:
Allows you to create users by sending their name and email.
Lets you fetch a list of all users from the database.
Uses PostgreSQL as the database, running inside Docker.
Uses async SQLAlchemy sessions for better performance.
Built with FastAPI so you get automatic API docs and fast development.

How it works:
The API has two main endpoints:
POST/users/ to add a new user.
GET/users/ to get a list of all users.
User data is stored in a PostgreSQL database.
Docker and Docker Compose are used to set up both the API and the database.
Pydantic models are used for data validation and serialization.

How to run it:
1. Make sure you have Docker installed on your machine.
2. Clone this repository.
3. Create a `.env` file with your database URL.
4. Run the below command in the project folder to start everything:
docker-compose up --build
5. The API will be available at: `http://localhost:8000`
6. You can check the automatic API docs at: `http://localhost:8000/docs`

Technologies used:
Python 3.11
FastAPI
SQLAlchemy (async)
PostgreSQL (Docker container)
Pydantic
Docker & Docker Compose
Uvicorn (ASGI server)

