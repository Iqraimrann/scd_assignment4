# 📚 Library Management System - REST API (Flask)

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
