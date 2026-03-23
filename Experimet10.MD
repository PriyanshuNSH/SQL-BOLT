# EXPERIMENT-10
## 01.Find the longest time that an employee has been at the studio.
 Query
~~~sql   
SELECT MAX(years_employed) AS max_years
FROM employees;
~~~

## 02.For each role, find the average number of years employed by employees in that role.
 Query
~~~sql   
SELECT role, AVG(years_employed) AS avg_years
FROM employees
GROUP BY role;
~~~

## 03.Find the total number of employee years worked in each building.
 Query
~~~sql   
SELECT building, SUM(years_employed) AS total_years
FROM employees
GROUP BY building;
~~~
