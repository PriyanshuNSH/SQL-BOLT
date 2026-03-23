# EXPERIMENT-12
## 01.Find the number of movies each director has directed.
 Query
~~~sql   
SELECT director, COUNT(*) AS movie_count
FROM movies
GROUP BY director;
~~~

## 02.Find the total domestic and international sales that can be attributed to each director. 
 Query
~~~sql   
SELECT movies.director,
       SUM(boxoffice.domestic_sales + boxoffice.international_sales) AS total_sales
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id
GROUP BY movies.director;
~~~