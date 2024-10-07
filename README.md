# Library Management System

## Overview
This is a simple Library Management System developed using Python. It allows administrators to manage books and members, and users to borrow or return books, pay fines, and view overdue books.

## Features
1. **Admin Features:**
   - Add, update books.
   - Add, update members.
   - View available books, members.
   - View issued and overdue books.

2. **User Features:**
   - View available books.
   - Borrow and return books.
   - Pay fines.

3. **Overdue Books:**
   - The system tracks borrowed books and calculates overdue fines based on a 14-day borrowing period.

4. **Fine Payment:**
   - Users can pay fines based on overdue returns.

## Running the Program

1. **Requirements:**
   - Python 3.x.
   - CSV files for books, members, and users (included in the repository).

2. **How to Run:**
   1. Download or clone the repository.
   2. Ensure the CSV files (`books.csv`, `members.csv`, `users.csv`) are in the same directory as the Python file.
   3. Run the Python script:
      ```bash
      python library_management.py
      ```
   4. You will be presented with the main menu:
      - Admin Login
      - User Login
      - Exit

3. **Admin Credentials:**
   - Default admin username: `admin`
   - Default admin password: `admin123`

4. **Test Case Verification:**
   - **Admin Functions:** Tested by adding, updating books and members.
   - **User Functions:** Tested by viewing books, issuing, and returning books.
   - **Overdue and Fine Calculation:** Validated by issuing books and returning them after the due period to check overdue fines.
   - **Fine Payment:** Tested by paying fines and verifying the updated balance.
