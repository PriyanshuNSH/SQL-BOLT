# EXPERIMENT-13
## 01.Add the studio's new production, Toy Story 4 to the list of movies (you can use any director).
 Query
~~~sql   
INSERT INTO movies
VALUES (NULL, 'Toy Story 4', 'John Lasseter', 2019, 100);
~~~

## 02.Toy Story 4 has been released to critical acclaim! It had a rating of 8.7, and made 340 million domestically and 270 million internationally. Add the record to the BoxOffice table.
 Query
~~~sql   
INSERT INTO boxoffice
VALUES (4, 8.7, 340000000, 270000000);
~~~