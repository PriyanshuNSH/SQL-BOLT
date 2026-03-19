# EXPERIMENT-3
# 01. Find all the Toy Story movies.
```sql
SELECT * FROM movies
WHERE title LIKE 'Toy Story%' ;
```
# 02.Find all the movies directed by John Lasseter
```sql
SELECT * FROM movies
WHERE director = 'John Lasseter'; 
```

# 03.Find all the movies (and director) not directed by John Lasseter
```sql
SELECT title , Director FROM movies
WHERE director <> 'John Lasseter';
```

# 04.Find all the WALL-* movies
```sql
SELECT * FROM movies
WHERE title LIKE 'WALL-%';
```