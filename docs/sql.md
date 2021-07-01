# SQL

Structured Query Language

## General

- Insert
```SQL
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...),
(value1, value2, value3, ...);
```

- Update
```SQL
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

- Delete
```SQL
DELETE FROM table_name WHERE condition;
```

## SQL Server

- Insert Chinese Data
When Chinese chatacters displays as "?", put "N" before the data can solve the issue.
```SQL
N'数据示例'
```
