# Aggregate Functions in SQL

Aggregate functions in SQL perform calculations on multiple rows of a table and return a single value. These functions are commonly used with the **GROUP BY** clause to group data into subsets for calculation.

## 1. MIN()
- Returns the smallest value in a column.
- **Example:**
  ```sql
  SELECT MIN(salary) AS MinimumSalary
  FROM employees;
  ```

## 2. MAX()
- Returns the largest value in a column.
- **Example:**
  ```sql
  SELECT MAX(salary) AS MaximumSalary
  FROM employees;
  ```

## 3. COUNT()
- Returns the number of rows in a column (excluding `NULL` values).
- Use `COUNT(*)` to include `NULL` values.
- **Example:**
  ```sql
  SELECT COUNT(employee_id) AS TotalEmployees
  FROM employees;
  ```

## 4. SUM()
- Returns the total sum of numeric values in a column.
- **Example:**
  ```sql
  SELECT SUM(salary) AS TotalSalaries
  FROM employees;
  ```

## 5. AVG()
- Returns the average (mean) value of a numeric column.
- **Example:**
  ```sql
  SELECT AVG(salary) AS AverageSalary
  FROM employees;
  ```

## 6. STDDEV()
- Returns the standard deviation of numeric values in a column.
- Measures how much data deviates from the mean.
- **Example:**
  ```sql
  SELECT STDDEV(salary) AS SalaryStandardDeviation
  FROM employees;
  ```

## 7. VARIANCE()
- Returns the variance of numeric values in a column.
- Measures the spread of data values.
- **Example:**
  ```sql
  SELECT VARIANCE(salary) AS SalaryVariance
  FROM employees;
  ```

---

## Notes
- Aggregate functions ignore `NULL` values by default (except `COUNT(*)`).
- To calculate these values for subsets of data, combine with the `GROUP BY` clause:
  ```sql
  SELECT department_id, AVG(salary) AS AverageSalary
  FROM employees
  GROUP BY department_id;
  
