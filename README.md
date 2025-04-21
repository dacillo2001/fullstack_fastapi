Full-Stack To-Do List Application

This project is a full-stack To-Do List application that integrates a React frontend with a FastAPI backend. The backend provides a RESTful API and uses SQLite for database storage, while the frontend allows users to add, edit, delete, and filter tasks.

*Setup Instructions
 Prerequisites
-Node.js and npm (for React frontend)
-Python (for FastAPI backend)
-SQLite (if not using the default setup)

*Frontend (FastAPI)

1.Clone the repository:
2.git clone <repository-url>
3.cd <repository-folder>
4.Install the frontend dependencies: npm install
5.Run the development server: npm run dev The frontend will be available at http://localhost:3000.

*Backend (React)
1.Navigate to the backend folder:
-cd fastapi-backend

2.Create and activate a virtual environment (for Python):
-python -m venv venv source venv/bin/activate # On Windows: venv\Scripts\activate

*Install the backend dependencies:

pip install -r requirements.txt

Run the FastAPI development server:

uvicorn app.main:app --reload The backend will be available at http://localhost:8000.

Backend API Endpoints:

GET https://nicoleback.onrender.com/nicoletodo/
Description: Fetch all to-do items.

1.POST https://nicoleback.onrender.com/nicoletodo/ Description: Create a new to-do item.

2.GET https://nicoleback.onrender.com/nicoletodo/%7Btodo_id%7D Description: Fetch a single to-do item by ID.

3.PUT https://nicoleback.onrender.com/nicoletodo/%7Btodo_id%7D Description: Update a to-do item by ID.

4.DELETE https://nicoleback.onrender.com/nicoletodo/%7Btodo_id%7D Description: Delete a to-do item by ID.

5.GET https://nicoleback.onrender.com/nicoletodo/filter/%7Bstatus%7D Description: Fetch to-do items filtered by status (completed or pending).
