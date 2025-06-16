SCD Assignment 04 – Flask REST API
Student Name: Iqra Imran
Roll Number: F2022065355
Course: Software Construction and Development (SCD) – Week 4
Assignment No: 04

📌 Objective
This assignment demonstrates how to implement a simple RESTful API using Flask and perform CRUD operations on an in-memory list of books. The project also includes steps to upload the code to GitHub and simple instructions for testing the endpoints.

📂 Project Structure
bash
Copy
Edit
scd_assignment4/
│
├── app.py             # Main Flask application
├── requirements.txt   # Dependencies
└── README.md          # Documentation (this file)
✅ Part 01 – Setup Flask REST API
🔧 Step-by-Step Instructions
Create a Virtual Environment:

bash
Copy
Edit
python -m venv venv
Activate the Environment:

On Windows:

bash
Copy
Edit
venv\Scripts\activate
On Mac/Linux:

bash
Copy
Edit
source venv/bin/activate
Install Flask:

bash
Copy
Edit
pip install Flask
Create a file app.py and write the Flask REST API code.

Run the Flask App:

bash
Copy
Edit
python app.py
✅ Part 02 – Book REST API Implementation
This API allows you to manage an in-memory list of books using simple CRUD operations.

🧾 Sample Book Data
python
Copy
Edit
books = [
    {"id": 1, "title": "The Alchemist", "author": "Paulo Coelho"},
    {"id": 2, "title": "Atomic Habits", "author": "James Clear"}
]
🔨 API Requirements
📘 Requirement 01: Add Book
Endpoint: POST /books

Adds a new book to the list.

📖 Requirement 02: View All Books
Endpoint: GET /books

Returns a list of all books.

🔍 Requirement 03: Search Book by Title
Endpoint: GET /books/<title>

Searches and returns book by title.

❌ Requirement 04: Delete Book by Title
Endpoint: DELETE /books/<title>

Deletes a book from the list by title.

💻 Execution Guide
1. GET /books – Get All Books
Request:

http
Copy
Edit
GET /books
Response:

json
Copy
Edit
[
  {"id": 1, "title": "The Alchemist", "author": "Paulo Coelho"},
  {"id": 2, "title": "Atomic Habits", "author": "James Clear"}
]
2. GET /books/<id> – Get Single Book by ID
Request:

http
Copy
Edit
GET /books/1
Response:

json
Copy
Edit
{"id": 1, "title": "The Alchemist", "author": "Paulo Coelho"}
3. POST /books – Add a New Book
Request:

json
Copy
Edit
{
  "title": "Rich Dad Poor Dad",
  "author": "Robert Kiyosaki"
}
Response:

json
Copy
Edit
{"message": "Book added successfully"}
4. DELETE /books/<id> – Delete Book by ID
Request:

http
Copy
Edit
DELETE /books/2
Response:

json
Copy
Edit
{"message": "Book deleted successfully"}
📎 GitHub Repository Link
🔗 GitHub Repository – SCD Assignment 4

📌 Notes
This app is built with Flask using in-memory storage (no database).

Make sure to install the required libraries before running the app.

For testing, you can use tools like Postman or curl.
This is a simple Library Management System REST API built using Python and Flask. It allows you to manage books — add them, and view all books.

## 📁 Folder Structure

library_api/
├── app.py
├── requirements.txt
├── README.md
├── models/
│   ├── Book.py
│   ├── Library.py
│   └── Student.py
└── routes/
    └── library_routes.py

## ▶️ How to Run the Project

1. Install Flask
```
pip install flask
```

2. Start the Flask Server
```
python app.py
```

3. Test in Postman
- `GET /books` → View all books
- `POST /books` → Add a new book
  JSON Example:
  {
    "title": "Python Basics",
    "author": "Iqra Imran",
    "isbn": "12345"
  }

## ✅ Features

- Add a book
- View all books

## 👩‍💻 Developed By

Iqra Imran (ID: 355)
For SCD Assignment 4 - REST API using Flask


