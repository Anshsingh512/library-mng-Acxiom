# Library Management System

## Overview

This is a console-based Library Management System that allows administrators and users to manage books, members, and issue/return records. The system includes features such as book issuance, overdue fine calculation, and basic CRUD operations for books and members. Data is stored in CSV files for persistence across sessions.

## Features

### Admin Features
- **Add Book:** Add new books to the library's collection.
- **Add Member:** Register new members to the library system.
- **Update Book:** Modify details about existing books (title, author, genre, copies).
- **Update Member:** Modify member details.
- **View Available Books:** Display all books currently available for issuance.
- **View Available Members:** Display all registered members.
- **View Issued Books:** Display a list of books that are currently issued to members.
- **View Overdue Books:** Display a list of overdue books and their associated fines.
- **Logout:** Exit the admin session and return to the main menu.

### User Features
- **View Available Books:** View all books currently available for issuance.
- **Issue Book:** Issue a book from the library (if available).
- **Return Book:** Return an issued book and, if applicable, check for overdue fines.
- **Pay Fine:** Pay any outstanding fines due to overdue books.
- **Logout:** Exit the user session and return to the main menu.

## System Requirements

- Python 3.7 or above
- CSV files for storing books, members, and users data

## Installation and Setup

1. Clone the repository or download the project files.
2. Ensure that the following CSV files are present in the same directory:
   - `books.csv`: Stores information about books.
   - `members.csv`: Stores information about members.
   - `users.csv`: Stores credentials for admin and user logins.
3. To run the application, open a terminal in the project directory and run:

    ```bash
    python library_management.py
    ```

## CSV File Format

### books.csv
- **Fields:** `book_id`, `title`, `author`, `genre`, `copies`
- Example:

    ```csv
    book_id,title,author,genre,copies
    101,The Catcher in the Rye,J.D. Salinger,Fiction,5
    102,1984,George Orwell,Dystopian,3
    ```

### members.csv
- **Fields:** `member_id`, `name`, `membership_type`, `fines`
- Example:

    ```csv
    member_id,name,membership_type,fines
    201,John Doe,Premium,0
    202,Jane Smith,Standard,5
    ```

### users.csv
- **Fields:** `username`, `password`
- Example:

    ```csv
    username,password
    admin,admin123
    user,user123
    ```

## Usage Instructions

### Main Menu

Upon launching the program, you'll be greeted with the following options:

```plaintext
Welcome to the Library Management System
1. Admin Login
2. User Login
3. Exit

Admin Login
To log in as an admin, use the following credentials (these are default and can be changed in users.csv):

Username: admin
Password: admin123
Once logged in, you can access the admin menu to perform various management tasks.

User Login
For users, you can log in with credentials defined in users.csv. Example:

Username: user
Password: user123
Users can view and issue books, return them, and pay fines if applicable.

## Credentials
The default credentials for the system are as follows:

#Admin Login:
Username: admin
Password: admin123
#User Login:
Username: user
Password: user123

#Additional users can be added by modifying the users.csv file with appropriate username and password pairs.

#Fine Calculation
A fine of $1 per day is imposed on books returned after 14 days.
Users can pay their fines from the user menu under the "Pay Fine" option.
Customization
You can modify the following files to customize the system:

books.csv: Add or modify book details.
members.csv: Register new members or update existing ones.
users.csv: Add new admin or user credentials.
#Future Improvements
Implement a GUI for easier interaction.
Add search and filter functionalities for books and members.
Enable email notifications for overdue books.

#License
This project is open-source and free to use for educational purposes.
