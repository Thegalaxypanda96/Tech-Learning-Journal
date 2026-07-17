# PostgreSQL Basics

**Source:** freeCodeCamp Relational Databases Certification  
**Platform:** freeCodeCamp  
**Database:** PostgreSQL  
**Environment:** GitHub Codespaces (Linux)

---

# Overview

These notes cover the basics of PostgreSQL and using the `psql` command-line interface to create and manage databases and tables.

---

# PostgreSQL

PostgreSQL is an open-source **Relational Database Management System (RDBMS)** used to create, store, manage, and query relational databases.

Unlike graphical database tools, PostgreSQL can be managed directly from the terminal using the `psql` command-line application.

---

# Connecting to PostgreSQL

Connect to the PostgreSQL server:

```bash
psql --username=freecodecamp --dbname=postgres
```

### Command Breakdown

| Part | Description |
|------|-------------|
| `psql` | Launches the PostgreSQL command-line interface |
| `--username=freecodecamp` | Connects using the `freecodecamp` user |
| `--dbname=postgres` | Connects to the default PostgreSQL database |

After connecting, the prompt changes:

```text
postgres=>
```

The prompt always displays the database you are currently connected to.

---

# Listing Databases

Display all databases:

```sql
\l
```

Example Output:

```text
postgres
template0
template1
first_database
second_database
```

---

# Creating Databases

Create a new database:

```sql
CREATE DATABASE first_database;
```

Create another database:

```sql
CREATE DATABASE second_database;
```

Verify the databases were created:

```sql
\l
```

---

# Connecting to a Database

Switch to another database:

```sql
\c second_database
```

Example Output:

```text
You are now connected to database "second_database" as user "freecodecamp".
```

The prompt changes to:

```text
second_database=>
```

Any tables you create will be created inside the currently connected database.

---

# Viewing Tables

Display the tables (relations) in the current database:

```sql
\d
```

If no tables exist, PostgreSQL displays:

```text
Did not find any relations.
```

---

# Creating Tables

Create a table:

```sql
CREATE TABLE first_table();
```

Create another table:

```sql
CREATE TABLE second_table();
```

Verify they were created:

```sql
\d
```

> **Note:** Even an empty table requires parentheses `()`.

---

# SQL Syntax

Every SQL statement ends with a semicolon (`;`).

Example:

```sql
CREATE DATABASE first_database;
```

If you forget the semicolon, PostgreSQL assumes the command is incomplete and waits for the rest of the statement.

You can simply type:

```sql
;
```

and press **Enter** to execute it.

---

# SQL Keywords

Keywords are reserved words that tell SQL what action to perform.

Examples:

- `CREATE`
- `DATABASE`
- `TABLE`
- `SELECT`
- `INSERT`
- `UPDATE`
- `DELETE`

Keywords are commonly written in uppercase for readability.

---

# PostgreSQL Meta Commands

Meta commands begin with a backslash (`\`) and are interpreted by the `psql` client instead of SQL itself.

| Command | Description |
|---------|-------------|
| `\l` | List all databases |
| `\c database_name` | Connect to a database |
| `\d` | Display tables (relations) in the current database |

---

# Key Concepts

## PostgreSQL

An open-source Relational Database Management System (RDBMS).

---

## Database

An organized collection of related data.

A PostgreSQL database contains tables and other database objects.

---

## Table

A table stores related information in rows and columns.

Example:

```text
Students
------------------------
ID | Name | Major
```

---

## Relation

In PostgreSQL, a **relation** is a database object.

Relations include:

- Tables
- Views
- Indexes
- Sequences

The `\d` command lists the relations in the current database.

---

## SQL

**Structured Query Language**

Used to create, retrieve, update, and manage data in relational databases.

---

## SQL Statement

An instruction executed by PostgreSQL.

Examples:

- `CREATE DATABASE`
- `CREATE TABLE`
- `SELECT`

---

## Semicolon (`;`)

Marks the end of an SQL statement.

Without a semicolon, PostgreSQL waits for the rest of the command.

---

# Workflow Learned

1. Connect to PostgreSQL.

```bash
psql --username=freecodecamp --dbname=postgres
```

2. List databases.

```sql
\l
```

3. Create a database.

```sql
CREATE DATABASE first_database;
```

4. Connect to a database.

```sql
\c second_database
```

5. Display tables.

```sql
\d
```

6. Create a table.

```sql
CREATE TABLE first_table();
```

7. Verify the table exists.

```sql
\d
```

---

# Commands Learned

| Command | Description |
|---------|-------------|
| `psql --username=freecodecamp --dbname=postgres` | Connect to PostgreSQL |
| `\l` | List all databases |
| `\c database_name` | Connect to a database |
| `\d` | Display tables (relations) |
| `CREATE DATABASE database_name;` | Create a new database |
| `CREATE TABLE table_name();` | Create a new table |
