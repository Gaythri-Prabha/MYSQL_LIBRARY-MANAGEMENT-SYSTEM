# MYSQL_LIBRARY-MANAGEMENT-SYSTEM
This project is a SQL-based relational database design for a Library Management System. The database structure includes tables to manage library branches, employees, books, customers, and book issuance and return statuses.

Database Structure
The database contains six main tables:

Branch: Stores information about each library branch, including branch number, manager ID, address, and contact number.

Employee: Contains details about library employees, such as employee ID, name, position, salary, and the branch they are assigned to.

Books: Maintains a catalog of books in the library, with details like ISBN, title, category, rental price, availability status, author, and publisher.

Customer: Tracks library members, including customer ID, name, address, and registration date.

IssueStatus: Logs details of book issuance to customers, including the issue ID, customer ID, book name, issue date, and ISBN of the book issued.

ReturnStatus: Tracks the return of issued books, including the return ID, customer ID, book name, return date, and ISBN of the book returned.

Table Relationships
Branch and Employee: Linked by Branch_no, establishing which branch an employee is assigned to.
Books, IssueStatus, and ReturnStatus: Linked by ISBN, tracking the book's availability and circulation.
Customer, IssueStatus, and ReturnStatus: Linked by Customer_Id, logging customer activity for issuing and returning books.
Example Usage
The database can be used in applications for:

Tracking library book inventory.
Monitoring book issuance and return transactions.
Managing library branches and employees.
Getting Started
To set up the database:

Create and use the library database.
Run the provided SQL script to create tables and define relationships.
