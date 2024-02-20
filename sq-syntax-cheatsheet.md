### 1. Basic Syntax:

```sql
SELECT column1, column2, ...
FROM table_name;
```

- `SELECT`: Keyword used to specify which columns you want to retrieve.
- `column1, column2, ...`: Names of the columns you want to retrieve. You can specify multiple columns separated by commas.
- `FROM`: Keyword used to specify the table from which you are retrieving data.
- `table_name`: Name of the table from which you want to retrieve data.

### 2. Example:

```sql
SELECT id, name, age, department
FROM employees;
```

- Retrieves the `id`, `name`, `age`, and `department` columns from the `employees` table.

### 3. Retrieving All Columns:

```sql
SELECT *
FROM employees;
```

- Retrieves all columns from the `employees` table.

### 4. Filtering Results:

```sql
SELECT *
FROM employees
WHERE department = 'HR';
```

- Retrieves all columns from the `employees` table where the `department` is `'HR'`.

### 5. Sorting Results:

```sql
SELECT *
FROM employees
ORDER BY age DESC;
```

- Retrieves all columns from the `employees` table and sorts the results by the `age` column in descending order (`DESC`).

### 6. Limiting Results:

```sql
SELECT *
FROM employees
LIMIT 10;
```

- Retrieves the first 10 rows from the `employees` table.

### 7. Aggregating Data:

```sql
SELECT COUNT(*)
FROM employees;
```

- Counts the number of rows in the `employees` table.

### 8. Grouping Data:

```sql
SELECT department, AVG(age) AS avg_age
FROM employees
GROUP BY department;
```

- Groups the data by the `department` column and calculates the average age (`AVG(age)`) for each department.

### 9. Combining Conditions:

```sql
SELECT *
FROM employees
WHERE department = 'HR' AND age > 30;
```

- Retrieves all columns from the `employees` table where the `department` is `'HR'` and the `age` is greater than `30`.

### 10. Aliasing Columns:

```sql
SELECT name AS employee_name, age AS employee_age
FROM employees;
```

- Retrieves the `name` column as `employee_name` and the `age` column as `employee_age` from the `employees` table.

### 11. Joining Tables:

```sql
SELECT e.name AS employee_name, d.name AS department_name
FROM employees e
JOIN departments d ON e.department_id = d.id;
```

- Retrieves the `name` column from the `employees` table aliased as `employee_name` and the `name` column from the `departments` table aliased as `department_name`. It joins the two tables based on the `department_id` in the `employees` table matching the `id` in the `departments` table.
