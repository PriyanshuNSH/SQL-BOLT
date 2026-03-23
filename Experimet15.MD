# EXPERIMENT-15
## 01.This database is getting too big, lets remove all movies that were released before 2005.
 Query
~~~sql   
DELETE FROM movies
WHERE year < 2005;
~~~

## 02.Andrew Stanton has also left the studio, so please remove all movies directed by him.
 Query
~~~sql   
DELETE FROM movies
WHERE director = 'Andrew Stanton';
~~~