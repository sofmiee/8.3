CREATE TABLE employees(
employee_id INT PRIMARY KEY,
name_ VARCHAR(100),
department VARCHAR(100),
salary INT,
hire_date DATE
);

INSERT INTO employees(employee_id, name_, department, salary, hire_date)
VALUES (1, 'Alice', 'HR', 70000, '2019-01-15'),
(2, 'Bob', 'IT', 90000, '2020-06-01'),
(3, 'Charlie', 'IT', 80000, '2021-03-10'),
(4, 'Diana', 'Marketing', 60000, '2022-11-25');

SELECT * FROM employees
WHERE hire_date > '2020-01-01'
ORDER BY salary DESC;
