# 📚 Library Management System (LMS)

## 🧾 Project Overview

This project showcases my ability to design and optimize relational databases using **SQL**, focusing on real-world problem-solving. It includes **data modeling**, **schema creation**, and the implementation of **advanced SQL queries** to manage library operations efficiently. I also emphasize **data integrity**, **query optimization**, and **scalability**.

---

## 🗃️ Database Schema

The LMS system is structured around core relational tables to manage data effectively:

| Table         | Description                                 |
| ------------- | ------------------------------------------- |
| authors       | Stores author information                   |
| books         | Contains book details                       |
| members       | Holds data on registered library users      |
| loans         | Tracks book borrow and return activity      |
| fines         | Records fines associated with overdue loans |
| book\_authors | Junction table for books and authors        |

### Entity Relationships

* One **Author** → Many **Books**
* One **Book** → Many **Authors**
* Many-to-Many relationship handled via **BookAuthors**
* One **Book** → Many **Loans**
* One **Member** → Many **Loans**
* One **Loan** → Zero or One **Fine**

---

## 🧱 Key Features

* **Relational Database Design**: Designed efficient schemas with normalization to prevent redundancy and ensure data consistency.
* **SQL Queries**: Wrote optimized SQL queries to extract insights, track book loans, calculate fines, and manage member activity.
* **Real-World Simulations**: Applied real-life scenarios like fine calculations and loan tracking to ensure that the system simulates actual operations.

---

## 🔍 Sample SQL Queries

### Basic Queries

* List all books and their authors.
* Display active (unreturned) loans.
* View registered library members.

### Advanced Queries

* **Top 3 Most Borrowed Books**: Optimized query for frequent loan queries.
* **Calculate Total Fines per Member**: Aggregated data to track overdue fines.
* **List Members Borrowing from Multiple Genres**: Query to identify members with diverse reading habits.

---

## 🛠️ Tools & Technologies

* **SQL** (Microsoft SQL Server Management Studio): Mastery in writing efficient queries for data extraction and manipulation.
* **ERD Tool** (MySQL Workbench): Created Entity-Relationship Diagrams to visualize and design the database schema.
* **Text Editor** (VS Code): Used for writing SQL scripts and managing the project structure.

---

## 📈 Key Takeaways

* **SQL Proficiency**: Expertise in using SQL for querying and database management.
* **Database Design**: Created normalized relational schemas, ensuring efficient data storage and retrieval.
* **Real-World Application**: Focused on implementing a system that could be practically used by libraries to manage operations.
* **Optimized Queries**: Wrote advanced SQL queries for real-time data analytics and reporting.

---

## 📁 Project Structure

```
library_management_system/
├── README.md                # A brief introduction and instructions on using the repository
├── /ddl-scripts             # Contains the schema creation scripts (e.g., CREATE TABLE statements)
│   └── create_tables.sql    # Script to create all database tables
│   └── alter_tables.sql     # Script for any alterations (if needed)
│
├── /data-inserts            # Contains the scripts for inserting data into tables
│   └── insert_authors.sql   # Script to insert randomized authors
│   └── insert_books.sql     # Script to insert randomized books
│   └── insert_loans.sql     # Script to insert randomized loans
│   └── insert_fines.sql     # Script to insert randomized fines
│
├── /queries-examples        # Contains example queries to demonstrate usage
│   └── query_loans.sql      # Example query to check loan records
│   └── query_fines.sql      # Example query for fines
│   └── query_books.sql      # Example query for books
│   └── query_members.sql    # Example query to check members' information
│
└── /documentation           # Additional documents, if any (e.g., project proposal, flowcharts)
    └── project_summary.md   # Overview and summary of the project
    └── database_diagram.png # Optional, diagram of the database schema

```

---

## 🧠 Future Improvements

* Add triggers for automatic fine calculation based on loan return dates.
* Create stored procedures for issuing and returning books.
* Implement user roles (admin, member) with different levels of access.
* Integrate with a web or Python-based front-end for a complete system.

---

## 👨‍💻 Author
**Kevin Costa**  
Data Scientist | Machine Learning Researcher | Python Developer | Scientific Computing

📫 dacosta.kevin.mota@gmail.com

🌐 https://www.linkedin.com/in/costakevinn/
