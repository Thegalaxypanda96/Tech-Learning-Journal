# SQL Tutorial Notes (freeCodeCamp)

## Databases

### Relational Databases
- Store data in **tables**

### Non-Relational Databases
Other ways to store data:
- Documents
- Graphs
- Nodes

Database management systems exist for both relational and non-relational databases.

---

## Queries

A **query** is a request for information from a database.

---

## Tables & Keys

### Relational Data
- Organized into **rows** and **columns**

### Primary Key
- Every table should have one primary key.
- A primary key uniquely identifies each row of data.
- A table can only have **one** primary key.

### Surrogate Key
- Has no real-world meaning.
- Usually a randomly generated number (such as an auto-incrementing ID).

### Natural Key
- Has a real-world meaning.
- Represents actual data (such as a Social Security Number or Employee ID).

### Foreign Key
- A key that references the primary key of another table.
- Creates relationships between tables.
- A table can have **multiple foreign keys**.

## Composite Key
A **composite key** is a key made up of **two or more columns** that together create a unique identifier for a table.

---

## SQL Basics

**SQL (Structured Query Language)** is used to interact with a Database Management System (DBMS).

Common uses include:
- Create data
- Retrieve data
- Update data
- Delete data
- Create and manage databases

---

## SQL

- SQL can vary slightly between database systems.
- SQL is a hybrid language.

### SQL Language Categories

- **DQL** – Data Query Language
- **DDL** – Data Definition Language
- **DCL** – Data Control Language
- **DML** – Data Manipulation Language

---

## Queries

Queries allow you to retrieve only the information you want.

Basic query keywords:
- `SELECT`
- `FROM`
- `WHERE`

## Common SQL Data Types

### `INT`
- Stores whole numbers.

### `DECIMAL(M, N)`
- Stores exact numeric values.
- `M` = Total number of digits.
- `N` = Number of digits after the decimal point.

### `VARCHAR(n)`
- Stores variable-length text.
- `n` specifies the maximum number of characters.

### `BLOB`
- Stores large binary objects such as images, files, or other binary data.

### `DATE`
- Stores dates in the format:
  - `YYYY-MM-DD`

### `TIMESTAMP`
- Stores both the date and time in the format:
  - `YYYY-MM-DD HH:MM:SS`
