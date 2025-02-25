# SQL Basic Concepts

## Introduction
SQL (Structured Query Language) is a standard programming language used for managing and manipulating relational databases. It allows you to create, read, update, and delete data in a structured and organized manner.

## Key Concepts

### 1. Database
A database is a collection of organized information that can be easily accessed, managed, and updated. In SQL, databases are used to store and retrieve data.

### 2. Table
A table is a collection of related data organized into rows and columns. Each row represents a single record, and each column represents a field within the record.

### 3. Schema
A schema is a logical container for database objects such as tables, views, and indexes. It defines the structure of the database.

### 4. SQL Commands
SQL commands can be categorized into the following types:

#### a. Data Definition Language (DDL)
- `CREATE`: Used to create database objects such as tables, indexes, and views.
- `ALTER`: Used to modify existing database objects.
- `DROP`: Used to delete database objects.

#### b. Data Manipulation Language (DML)
- `SELECT`: Used to retrieve data from one or more tables.
- `INSERT`: Used to add new records to a table.
- `UPDATE`: Used to modify existing records in a table.
- `DELETE`: Used to remove records from a table.

#### c. Data Control Language (DCL)
- `GRANT`: Used to provide access privileges to users.
- `REVOKE`: Used to remove access privileges from users.

#### d. Transaction Control Language (TCL)
- `COMMIT`: Used to save changes made during a transaction.
- `ROLLBACK`: Used to undo changes made during a transaction.
- `SAVEPOINT`: Used to set a point within a transaction to which you can later roll back.

## Basic SQL Queries

### 1. Creating a Table
```sql
CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    email VARCHAR(100),
    hire_date DATE
);
```

### 2. Inserting Data
```sql
INSERT INTO employees (employee_id, first_name, last_name, email, hire_date)
VALUES (1, 'John', 'Doe', 'john.doe@example.com', '2023-01-15');
```

### 3. Selecting Data
```sql
SELECT * FROM employees;
```

### 4. Updating Data
```sql
UPDATE employees
SET email = 'john.doe_updated@example.com'
WHERE employee_id = 1;
```

### 5. Deleting Data
```sql
DELETE FROM employees
WHERE employee_id = 1;
```

## SQL Functions

### 1. Aggregate Functions
- `COUNT()`: Returns the number of rows.
- `SUM()`: Returns the sum of a numeric column.
- `AVG()`: Returns the average value of a numeric column.
- `MIN()`: Returns the minimum value of a column.
- `MAX()`: Returns the maximum value of a column.

### 2. String Functions
- `CONCAT()`: Concatenates two or more strings.
- `SUBSTRING()`: Extracts a substring from a string.
- `UPPER()`: Converts a string to uppercase.
- `LOWER()`: Converts a string to lowercase.
- `LENGTH()`: Returns the length of a string.

### 3. Date Functions
- `NOW()`: Returns the current date and time.
- `CURDATE()`: Returns the current date.
- `CURTIME()`: Returns the current time.
- `DATE_ADD()`: Adds a specified interval to a date.
- `DATE_SUB()`: Subtracts a specified interval from a date.

## Conclusion
SQL is a powerful language for managing and manipulating relational databases. Understanding the basic concepts and commands of SQL will help you efficiently work with databases and perform various data operations.
