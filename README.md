# Task-3
Extract data from one or more tables

Deliverables:SQL script with SELECT, WHERE, ORDER BY, LIMIT  

1.Use SELECT * and specific columns 
2.Apply WHERE, AND, OR, LIKE, BETWEEN
3.Sort with ORDER BY

Outcome: Clear understanding of how to retrieve data



-- 1. SELECT all columns from the employees table
SELECT * FROM employees;

-- 2. SELECT specific columns (name, department, salary)
SELECT name, department, salary FROM employees;

-- 3. Use WHERE to filter employees in the IT department
SELECT * FROM employees
WHERE department = 'IT';

-- 4. Use WHERE with AND to filter employees in IT department and salary above 70000
SELECT * FROM employees
WHERE department = 'IT' AND salary > 70000;

-- 5. Use WHERE with OR to find employees in HR or aged above 40
SELECT * FROM employees
WHERE department = 'HR' OR age > 40;

-- 6. Use LIKE to find employees whose names start with 'J'
SELECT * FROM employees
WHERE name LIKE 'J%';

-- 7. Use BETWEEN to find employees aged between 30 and 40
SELECT * FROM employees
WHERE age BETWEEN 30 AND 40;

-- 8. Use ORDER BY to sort employees by salary in descending order
SELECT * FROM employees
ORDER BY salary DESC;

-- 9. Use ORDER BY to sort employees by name alphabetically
SELECT * FROM employees
ORDER BY name ASC;

-- 10. Use LIMIT to get top 3 highest paid employees
SELECT * FROM employees
ORDER BY salary DESC
LIMIT 3;



