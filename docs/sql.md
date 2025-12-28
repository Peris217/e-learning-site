# SQL – Learning Documentation

## What SQL Is
SQL (Structured Query Language) is a language used to interact with databases.
It allows us to store, retrieve, update, and delete data in a structured way.

## Why I Am Learning SQL
- SQL is used in most web applications
- It is essential for backend development
- It is important for cybersecurity (databases often store sensitive data)
- Helps understand how applications handle data

## Core Concepts
- Database: A collection of structured data
- Table: Stores data in rows and columns
- Row (Record): One entry in a table
- Column (Field): A specific piece of data (e.g. username, email)

## Common SQL Commands
- SELECT – retrieve data from a table
- INSERT – add new data
- UPDATE – modify existing data
- DELETE – remove data
- WHERE – filter data
- ORDER BY – sort results
- LIMIT – restrict number of results

## Example Queries

```sql
-- Get all data from a table
SELECT * FROM users;

-- Get specific columns
SELECT username, email FROM users;

-- Filter results
SELECT * FROM users WHERE id = 1;

-- Insert new data
INSERT INTO users (username, email)
VALUES ('admin', 'admin@example.com');

-- Update existing data
UPDATE users
SET email = 'new@example.com'
WHERE id = 1;

-- Delete data
DELETE FROM users WHERE id = 1;