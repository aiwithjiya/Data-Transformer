# DataTransformer

## 📌 Project Overview

**DataTransformer** is a MySQL database project designed to demonstrate different SQL concepts such as **JOINs, Subqueries, Date Functions, String Functions, Window Functions, CASE Statements, and Data Transformation techniques**.

The project contains three main tables:

* Customers
* Orders
* Employees

It also includes **17 SQL queries** for retrieving, transforming, analyzing, and presenting data.

---

## 🗄️ Database

**Database Name:** `DataTransformer`

```sql
CREATE DATABASE DataTransformer;
USE DataTransformer;
```

---

## 📊 Database Tables

### 1. Customers

Stores customer information.

| Column           | Data Type    | Description                |
| ---------------- | ------------ | -------------------------- |
| CustomerID       | INT          | Unique customer ID         |
| FirstName        | VARCHAR(50)  | Customer first name        |
| LastName         | VARCHAR(50)  | Customer last name         |
| Email            | VARCHAR(100) | Customer email             |
| RegistrationDate | DATE         | Customer registration date |

---

### 2. Orders

Stores customer order information.

| Column      | Data Type     | Description        |
| ----------- | ------------- | ------------------ |
| OrderID     | INT           | Unique order ID    |
| CustomerID  | INT           | Customer reference |
| OrderDate   | DATE          | Date of order      |
| TotalAmount | DECIMAL(10,2) | Total order amount |

**Relationship:**

`Orders.CustomerID` → `Customers.CustomerID`

---

### 3. Employees

Stores employee information.

| Column     | Data Type     | Description          |
| ---------- | ------------- | -------------------- |
| EmployeeID | INT           | Unique employee ID   |
| FirstName  | VARCHAR(50)   | Employee first name  |
| LastName   | VARCHAR(50)   | Employee last name   |
| Department | VARCHAR(50)   | Employee department  |
| HireDate   | DATE          | Employee hiring date |
| Salary     | DECIMAL(10,2) | Employee salary      |

---

## 🔍 SQL Queries Included

### Query 1 – INNER JOIN

Retrieves orders along with their corresponding customer details.

### Query 2 – LEFT JOIN

Retrieves all customers and their corresponding orders.

### Query 3 – RIGHT JOIN

Retrieves all orders and their corresponding customers.

### Query 4 – FULL OUTER JOIN

Retrieves all customers and all orders using `LEFT JOIN`, `RIGHT JOIN`, and `UNION`.

### Query 5 – Subquery

Finds customers who placed orders above the average order amount.

### Query 6 – Subquery

Finds employees whose salary is above the average salary.

### Query 7 – Extract Year and Month

Extracts the year and month from `OrderDate`.

### Query 8 – Date Difference

Calculates the number of days between the order date and the current date.

### Query 9 – Date Formatting

Formats the order date into `DD-MMM-YYYY` format.

### Query 10 – Concatenate Name

Combines `FirstName` and `LastName` to create a full name.

### Query 11 – Replace String

Replaces `John` with `Jonathan`.

### Query 12 – Uppercase and Lowercase

Converts first names to uppercase and last names to lowercase.

### Query 13 – TRIM

Removes extra spaces from email values.

### Query 14 – Running Total

Calculates the cumulative running total of order amounts.

### Query 15 – Ranking

Ranks orders according to their total amount.

### Query 16 – CASE Statement

Assigns discounts based on the order amount.

| Total Amount | Discount    |
| ------------ | ----------- |
| > 1000       | 10% OFF     |
| > 500        | 5% OFF      |
| <= 500       | No Discount |

### Query 17 – Salary Category

Categorizes employees based on salary.

| Salary   | Category |
| -------- | -------- |
| >= 65000 | High     |
| >= 50000 | Medium   |
| < 50000  | Low      |

---

## 🛠️ Technologies Used

* **MySQL**
* **SQL**
* **MySQL Workbench / VS Code**
* Relational Database Concepts

---

## 📚 SQL Concepts Covered

* Database Creation
* Table Creation
* Primary Key
* Foreign Key
* INSERT
* SELECT
* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* FULL OUTER JOIN using UNION
* Subqueries
* Aggregate Functions
* `AVG()`
* `SUM()`
* Date Functions
* `YEAR()`
* `MONTH()`
* `DATEDIFF()`
* `DATE_FORMAT()`
* String Functions
* `CONCAT()`
* `REPLACE()`
* `UPPER()`
* `LOWER()`
* `TRIM()`
* Window Functions
* `RANK()`
* Running Total
* `CASE` Statements

---

## ▶️ How to Run

### Step 1: Open MySQL

Open **MySQL Workbench** or connect MySQL with **VS Code**.

### Step 2: Open the SQL File

Open the project `.sql` file containing the database, tables, data, and queries.

### Step 3: Execute the Script

Run the complete SQL script.

The script will:

1. Create the database.
2. Create all three tables.
3. Insert sample data.
4. Execute 17 SQL queries.
5. Display the results.

---

## 📁 Project Structure

```text
DataTransformer/
│
├── DataTransformer.sql
└── README.md
```

---

## 🎯 Project Objective

The main objective of this project is to practice and demonstrate SQL data transformation and analysis techniques using a relational database.

This project is useful for learning:

* Database Management
* SQL Query Writing
* Data Analysis
* Data Transformation
* Relational Database Operations

---

## ⭐ Conclusion

The **DataTransformer** project demonstrates how SQL can be used to retrieve, transform, analyze, and organize relational data efficiently using different SQL techniques and functions.

---

## 👩‍💻 Author

**Jiya Patel**
