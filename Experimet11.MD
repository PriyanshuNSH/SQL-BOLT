# EXPERIMENT-11
## 01.Find the number of Artists in the studio (without a HAVING clause).
 Query
~~~sql   
SELECT COUNT(*) AS artist_count
FROM employees
WHERE role = 'Artist';
~~~

## 02.Find the number of Employees of each role in the studio.
 Query
~~~sql   
SELECT role, COUNT(*) AS employee_count
FROM employees
GROUP BY role;
~~~

## 03.Find the total number of years employed by all Engineers.
 Query
~~~sql   
SELECT SUM(years_employed) AS total_years
FROM employees
WHERE role = 'Engineer';
~~~