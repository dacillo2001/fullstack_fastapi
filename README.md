Full-Stack To-Do List Application
This project is a full-stack To-Do List application that integrates a React frontend with a FastAPI backend. The backend provides a RESTful API and uses SQLite for database storage, while the frontend allows users to add, edit, delete, and filter tasks.

Setup Instructions
Prerequisites
Node.js and npm (for React frontend)
Python (for FastAPI backend)
SQLite (if not using the default setup)
Frontend (FastAPI)
Clone the repository:
git clone <repository-url>
cd <repository-folder>
Install the frontend dependencies: npm install
Run the development server: npm run dev The frontend will be available at http://localhost:3000.
Backend (React)
Navigate to the backend folder:

cd fastapi-backend

2.Create and activate a virtual environment (for Python):

python -m venv venv source venv/bin/activate # On Windows: venv\Scripts\activate

Install the backend dependencies:

pip install -r requirements.txt

Run the FastAPI development server:

uvicorn app.main:app --reload The backend will be available at http://localhost:8000.

Backend API Endpoints:

GET https://backendfastapi-rdsf.onrender.com/todos/
Description: Fetch all to-do items.

POST https://backendfastapi-rdsf.onrender.com/todos/ Description: Create a new to-do item.

GET https://backendfastapi-rdsf.onrender.com/todos/{todo_id} Description: Fetch a single to-do item by ID.

PUT https://backendfastapi-rdsf.onrender.com/todos/{todo_id} Description: Update a to-do item by ID.

DELETE https://backendfastapi-rdsf.onrender.com/todos/{todo_id} Description: Delete a to-do item by ID.

GET https://backendfastapi-rdsf.onrender.com/todos/filter/{status} Description: Fetch to-do items filtered by status (completed or pending).
