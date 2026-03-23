# EXPERIMENT-7
## 01.Find the list of all buildings that have employees.
 Query
~~~sql   
SELECT DISTINCT buildings.building_name
FROM buildings
INNER JOIN employees
ON buildings.building_name = employees.building;
~~~

## 02.Find the list of all buildings and their capacity.
 Query
~~~sql   
SELECT building_name, capacity
FROM buildings;
~~~

## 03.List all buildings and the distinct employee roles in each building (including empty buildings).
 Query
~~~sql   
SELECT DISTINCT buildings.building_name, employees.role
FROM buildings
LEFT JOIN employees
ON buildings.building_name = employees.building;
~~~