📘 FastAPI User Management Project

Welcome to the User Management API project! This project is a full-featured API built with FastAPI, providing endpoints to manage user data, including creating, reading, updating, and deleting users. This README will guide you through the setup, features, and code structure to help you get started quickly.

🚀 Project Features

	•	Create new users with names and email addresses.
	•	Read existing users or fetch user details by ID.
	•	Update user information such as name and email.
	•	Delete users by ID.
	•	Interactive Frontend to manage users visually.

 📂 Project Structure
 FastAPI User Management Project
├── Fast API/
│   ├── main.py           # FastAPI app entry point
│   ├── models.py         # SQLAlchemy models for User data
│   ├── schemas.py        # Pydantic schemas for data validation
│   ├── crud.py           # CRUD operations
│   ├── database.py       # Database configuration
├── templates/            # HTML templates (including the main frontend HTML)
└── README.md             # Project documentation

🔧 Setup Instructions

Prerequisites

	•	Ensure you have Python 3.7+ installed.
	•	Install FastAPI, SQLAlchemy, and Uvicorn for running the project.
 # Install dependencies
pip install fastapi sqlalchemy uvicorn
pip install python-dotenv  # To manage environment variables

Environment Setup

  1.	Create a .env file in the project root and define the database URL:
 DATABASE_URL=sqlite:///./test.db  # SQLite in local project folder

  2.	Update DATABASE_URL as per your database configuration if using PostgreSQL or MySQL.

Running the Project 🚀

	1.	Start the FastAPI server:
 uvicorn main:app --reload
 	2.	Open your browser at http://127.0.0.1:8000 to access the API.
	3.	Go to http://127.0.0.1:8000/docs to interact with the Swagger UI provided by FastAPI.

 🗂️ Code Structure Explanation

Main API Components

File	Purpose
main.py	Configures FastAPI app, routes, and endpoints for handling user CRUD operations.
models.py	Defines SQLAlchemy models for the User table.
schemas.py	Defines Pydantic schemas to validate request and response data.
crud.py	Contains CRUD functions for database interaction, handling user data operations.
database.py	Sets up database connection and session management using SQLAlchemy.

💻 Frontend Interface

index.html

A simple HTML interface for managing users through the following features:
	•	Create User: Input fields for name and email.
	•	Update User: Form to enter an ID and updated information.
	•	Delete User: Form to delete a user by ID.
	•	User List: A dynamic table showing all users with options to refresh.
