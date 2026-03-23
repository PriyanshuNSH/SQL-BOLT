# EXPERIMENT-6
## 01.Find the domestic and international sales for each movie.
 Query
~~~sql   
SELECT title, domestic_sales, international_sales
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id;
~~~

## 02.Show the sales numbers for each movie that did better internationally rather than domestically.
 Query
~~~sql   
SELECT movies.title, boxoffice.domestic_sales, boxoffice.international_sales
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id
WHERE boxoffice.international_sales > boxoffice.domestic_sales;
~~~

## 03.List all the movies by their ratings in descending order.
 Query
~~~sql   
SELECT movies.title, boxoffice.rating
FROM movies
INNER JOIN boxoffice
ON movies.id = boxoffice.movie_id
ORDER BY boxoffice.rating DESC;
~~~

