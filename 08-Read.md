# Reading 08 Notes

[Home](README.md)

# SQL
- Selecting query for specific columns
SELECT column, another_column, ...
FROM mytable;

- Selecting query for all columns
SELECT *
FROM mytable;

- Selecting query with constraints
SELECT column, another_column, ...
FROM mytable
WHERE *condition*
  AND/OR *another_condition*
  AND/OR ...;

|      Operator           |         Condition                                        | SQL Example                           |
|:------------------------|:--------------------------------------------------------:|--------------------------------------:|
| =, !=, < <=, >, >=      | Standard numerical operators                             | col_name !=4                          |
| BETWEEN ...AND ...      | Number is within range of two values (inclusive)         | col_name **BETWEEN** 1.5 **AND** 10.5 |
| NOT BETWEEN ... AND ... |Number is not within range of two values (inclusive)      | col_name **NOT BETWEEN** 1 **AND** 10 |
|      IN (...)           | Number exists in a list                                  | col_name **IN** (1,4,6)               |
|    NOT IN (...)         | Number does not exist in a list                          | col_name **NOT IN** (1,3,5)           |


SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;

## Filtering and sorting Query results
Select query with unique results:

- SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);

- Select query with ordered results:
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;

- Select query with limited rows:
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;

## Simple SELECT Queries
- SELECT query: 
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;

## Multi-table queries with JOINs
- Select query with INNER JOIN on multiple tables
SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;

