# EXPERIMENT-14
## 01.The director for A Bug's Life is incorrect, it was actually directed by John Lasseter.
 Query
~~~sql   
UPDATE movies
SET director = 'John Lasseter'
WHERE title = "A Bug's Life";
~~~

## 02.The year that Toy Story 2 was released is incorrect, it was actually released in 1999. 
 Query
~~~sql   
UPDATE movies
SET year = 1999
WHERE title = 'Toy Story 2';
~~~

## Q3.Both the title and director for Toy Story 8 is incorrect! The title should be "Toy Story 3" and it was directed by Lee Unkrich.
 Query
~~~sql
UPDATE movies
SET title = 'Toy Story 3',
    director = 'Lee Unkrich'
WHERE title = 'Toy Story 8';
~~~