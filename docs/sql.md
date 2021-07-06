# SQL

Structured Query Language

## General

- Insert
```sql
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...),
(value1, value2, value3, ...);

INSERT INTO Table_name
Select * FROM Another_TableName WHERE Condition
```

- Update
```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

- Delete
```sql
DELETE FROM table_name WHERE condition;
```
## Search

LIKE
```sql
-- 1. start with c
SELECT *
FROM student
WHERE name LIKE 'C%';
 
-- 2.end with n
SELECT *
FROM student
WHERE name LIKE '%n';
 
-- 3.have o in name
SELECT *
FROM student
WHERE name LIKE '%o%';
 
-- "_" repersent one char
 
-- 4.start with T and have 4 chars
SELECT *
FROM student
WHERE name LIKE 'T___';
```

## SQL Server

- Insert Chinese Data
When Chinese chatacters displays as "?", put "N" before the data can solve the issue.
```SQL
N'数据示例'
```
