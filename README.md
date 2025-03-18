# Library Management System

This project is a simple library management system built using Flask, SQLAlchemy, and SQLite. It allows users to borrow and return books, view books, and manage users. The system also uses enums to define different loan durations for books.

## Features

- **User Management**: Add new users and fetch existing users.
- **Book Management**: Add, update, delete, and view books in the library.
- **Borrowing System**: Users can borrow books for a specified duration, and the system calculates the return date based on the loan type (short, medium, or long).
- **Return System**: Users can return books, marking them as available again.

## Technologies Used

- **Flask**: Web framework used for the backend.
- **SQLAlchemy**: ORM for interacting with the SQLite database.
- **Flask-CORS**: To enable Cross-Origin Resource Sharing for frontend requests.
- **Flask-Migrate**: To handle database migrations.
- **Enum**: For defining different loan durations.

## Setup Instructions

### Prerequisites

Make sure you have Python 3.6+ installed. You will also need to install the required dependencies.

### Installation

1. Clone the repository:

   git clone https://github.com/HCHIX24/bib_back.git
   cd backend_bib
   #  " pip install -r requirements.txt "
# The application will be available at http://127.0.0.1:5000/
## Endpoints
GET /test: A simple test route to check if the server is running.
POST /books: Add a new book.
GET /books: Retrieve all books.
PUT /books/<int:book_id>: Update an existing book's details.
DELETE /books/<int:book_id>: Delete a book.
POST /users: Add a new user.
GET /users: Get all users.
POST /borrow: Borrow a book (requires user_id, book_id, and loan_type).
POST /return: Return a borrowed book (requires user_id and book_id).
DELETE /return: Return a borrowed book (alternative method).
## Contributions
Feel free to fork the repository and submit pull requests for any changes, improvements, or bug fixes.
