# SQL - Structured Query Language

## What is it, and why do we use it?

- database language - a language for manipulating and managing a database
- first developed in the 1970s
- SQL, Sqlite3, Postgresql, MySQL
- SQL is good for relational databases - in other words, handling/storing/retrieving data that's related

## Basic high-level structure of a database

- database itself - the whole database; one or more tables
- tables - a representation of a model - concrete or abstract
- schema - outline, or snapshot of the current structure of your database tables

## Basic commands

- what does CRUD mean?

  **C**reate
  **R**ead
  **U**pdate
  **D**elete

  These are the four basic actions we can take with data.

- how do we create a database?
```bash
sqlite3 countries
```

- how do we create a table?
```sql
CREATE TABLE countries (
  id INTEGER PRIMARY KEY,
  name TEXT,
  population INTEGER,
  capital TEXT,
);
```

- how do we change the structure of an existing table?
```sql
ALTER TABLE countries ADD COLUMN capital TEXT;
```

- how do we add data into a table?
```sql
INSERT INTO countries (name, capital, population) VALUES ("USA", "DC", 350000000);
```

- how do we edit existing rows in a table?
```sql
UPDATE countries SET capital = "Washington, DC" WHERE id = 1;
```

- how do we retrieve data from a table?
```sql
SELECT * FROM countries;
SELECT * citizens WHERE country_id = 2;
```
