# Chapter 4 - Structured Query Language

## 1. SELECT Statement
Retrieves data from one or more tables.

**Syntax**:  
```sql
SELECT column1, column2 
FROM table_name 
WHERE condition;
```

**Example**:  
```sql
SELECT first_name, last_name
FROM employees
WHERE department_id = 10;
```

To select all column in a table.

**Syntax**:  
```sql
SELECT * 
FROM table_name 
WHERE condition;
```

**Example**:  
```sql
SELECT *
FROM employeee;
```

## 2. INSERT Statement
Adds new rows to a table.

**Syntax**:  
```sql
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);
```
**Example**:  
```sql
INSERT INTO employees (first_name, last_name)
VALUES ('John', 'Doe');
```

## 3. UPDATE Statement

Modifies existing data within a table.

**Syntax**:  
```sql
UPDATE table_name
SET column1 = value1
WHERE condition;
```

**Example**:  
```sql
UPDATE employees
SET salary = 5000
WHERE employee_id = 1;
```

## 4. DELETE Statement

Removes rows from a table.

**Syntax**:  
```sql
DELETE FROM table_name
WHERE condition;
```

**Example**:  
```sql
DELETE FROM employees
WHERE employee_id = 1;
```

## 5. JOIN Clauses

Combines rows from two or more tables based on related columns.

**Example**:  
```sql
SELECT e.first_name, d.department_name
FROM employees e JOIN departments d
ON e.department_id = d.department_id;
```

## 6. GROUP BY Clause

Groups rows that have the same values in specified columns into summary rows.

**Syntax**:  
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
GROUP BY column1;
```

**Example**:  
```sql
SELECT department_id, COUNT(employee_id)
FROM employees
GROUP BY department_id;
```

## 7. HAVING Clause

Used with the GROUP BY clause to filter groups based on a condition (aggregate function).

**Syntax**:  
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
GROUP BY column1
HAVING condition;
```

**Example**:  
```sql
SELECT department_id, COUNT(employee_id)
FROM employees
GROUP BY department_id
HAVING COUNT(employee_id) > 5;
```

## 8. ORDER BY Clause

Sorts the result set in ascending or descending order.

**Syntax**:  
```sql
SELECT column1, column2
FROM table_name
ORDER BY column1 ASC|DESC;
```

**Example**:  
```sql
SELECT first_name, last_name
FROM employees
ORDER BY first_name ASC;
```

