# EXPERIMENT-9
## 01.List all movies and their combined sales in millions of dollars.
 Query
~~~sql   
SELECT movies.title,
       (boxoffice.domestic_sales + boxoffice.international_sales) / 1000000 AS total_sales_millions
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id;
~~~

## 02.List all movies and their ratings in percent.
 Query
~~~sql   
SELECT movies.title,
       boxoffice.rating * 10 AS rating_percent
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id;
~~~

## 03.List all movies that were released on even number years.
 Query
~~~sql   
SELECT title
FROM movies
WHERE year % 2 = 0;
~~~