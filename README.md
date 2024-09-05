Book DB
Book DB is a desktop-based application that allows users to manage a collection of books using a user-friendly interface.
Built with Python's Tkinter library for the frontend and MySQL Workbench for the backend, this project enables users to
perform CRUD operations on a book database.

Features
•	Add Books: Users can input book details (title, author, genre, and publication year) and add them to the database.
•	View Books: Display a list of all books stored in the MySQL database.
•	Update Books: Modify book information directly from the interface.
•	Delete Books: Remove books from the database when necessary.
•	Search Books: Search the database by title, author, or genre.
•	Database Integration: Uses MySQL for managing book records efficiently.

Tech Stack
•	Python: Core programming language.
•	Tkinter: GUI library used to build the desktop interface.
•	MySQL Workbench: Used as the database to store book information.
•	Pymysql: Python library to interact with the MySQL database.

Getting Started
Prerequisites
Before running the project, ensure you have the following installed:
•	Python 3.x
•	Tkinter (included with Python)
•	MySQL Workbench (and MySQL server)
•	Pymysql (Install using pip):


pip install pymysql
Setting Up the Virtual Environment
1.	Create a virtual environment: Navigate to your project directory and create a virtual environment using:
python -m venv venv

3.	Activate the virtual environment:
o	On Windows:
venv\Scripts\activate

o	On Mac/Linux:
source venv/bin/activate

3.	Install required dependencies: Install the necessary Python libraries within the virtual environment:
pip install pymysql

Setting Up the Database
1.	Open MySQL Workbench and create a new database for the project:
sql

CREATE DATABASE bookdb;

2.	Create a table to store book records:
sql

CREATE TABLE books (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    author VARCHAR(255) NOT NULL,
    genre VARCHAR(100),
    year INT
);

3.	Update the database connection details in your Python code (username, password, and database name).
Running the Application

1.	Clone the repository:
git clone https://github.com/Gaurav-Bansode-07/book-db.git

3.	Navigate to the project directory:
cd book-db

3.	Activate the virtual environment:
o	On Windows:
venv\Scripts\activate

o	On Mac/Linux:
source venv/bin/activate

4.	Run the application:
python app.py

