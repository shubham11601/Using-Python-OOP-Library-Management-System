# Using-Python-OOP-Library-Management-System

## 1. Overview

This project is a simple Library Management System built using Object-Oriented Programming (OOP) in Python.
It allows the library to manage books, register members, track borrowing and returning of books, and search for books by title.
The system is designed to mimic a real-world library process, but in a simplified form.
It’s a console-based application — perfect for learning OOP concepts like classes, objects, encapsulation, and methods.

## 2. Core Features

### a) Book Management

- Add new books to the library.
- View all books along with their availability status (Available / Borrowed).
- Each book stores:

- Title
- Author
- ISBN (unique identifier)
- Borrowed status

### b) Member Management

- Register new members to the library.
- Track each member's borrowed books.
- Limit of 3 books per member at a time.

### c) Borrowing & Returning Books

- Members can borrow books if:
- They haven’t reached the 3-book limit.
- The book is available.
- Members can return books they have borrowed.
- Automatically updates the book’s availability status.

### d) Search Functionality

- Search for books by title (case-insensitive).
- Returns all matching books.

## 3. Classes in the Project

### Book

- Represents a single book in the library.
- Attributes: title, author, ISBN, is_borrowed.
- Method: __str__() to display book info neatly.

### Member

- Represents a library member.
- Attributes: name, member_id, borrowed_books list.

### Methods:

- borrow_book(book) → borrow a book with rules.
- return_book(book) → return a borrowed book.

### Library

- Represents the whole library system.
- Attributes: books list, members list.

### Methods:

- add_book(book) → add a book to the library.
- display_all_books() → show all books.
- register_member(member) → add a new member.
- find_book_by_title(title) → search books.

## 4. How It Works

- The library is created.
- Books are added into the library’s collection.
- Members are registered.
- A member can:
- Borrow available books.
= Return borrowed books.
- The library can search for a book by title.
- The system updates and displays book status after each action.

## 5. Learning Outcomes

- OOP Concepts in Python:
- Class creation
- Object instantiation
- Attributes & methods
- Encapsulation & state management
- Working with lists to store and manage collections.
- Implementing business rules (max borrow limit, status checks).
- Using search/filter logic in Python.

## 6. Possible Enhancements

- Save and load data to/from files (CSV, JSON, or database).
- Add a due date and calculate fines for late returns.
- Create a menu-driven interactive CLI.
- Build a GUI with Tkinter or PyQt for better usability.
