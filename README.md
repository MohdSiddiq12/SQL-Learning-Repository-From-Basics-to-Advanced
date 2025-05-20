# SQL Learning Exercises

A comprehensive collection of SQL exercises to practice and improve your database skills.

## Table of Contents
- [Overview](#overview)
- [Getting Started](#getting-started)
- [Exercise Categories](#exercise-categories)
  - [1. Basic SQL Queries](#1-basic-sql-queries)
  - [2. Filtering and Sorting](#2-filtering-and-sorting)
  - [3. Joins and Relationships](#3-joins-and-relationships)
  - [4. Aggregations and Grouping](#4-aggregations-and-grouping)
  - [5. Data Modification](#5-data-modification)
  - [6. Subqueries and Complex Queries](#6-subqueries-and-complex-queries)
  - [7. Advanced SQL Techniques](#7-advanced-sql-techniques)
  - [8. Performance and Optimization](#8-performance-and-optimization)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository contains SQL exercises designed to help you learn and practice SQL concepts from basic to advanced levels. Each exercise includes a task description and expected outcome to guide your learning.

## Getting Started

1. Clone this repository to your local machine
2. Set up a MySQL or compatible database
3. Run the database schema setup script
4. Work through exercises in your preferred order
5. Check solutions only after attempting the exercises yourself

## Exercise Categories

### 1. Basic SQL Queries

**Task 1: Select all data from the bands table**

[1.Solution](#1-Solutions\1)

Expected Outcome:
```
| id | name            |
|----|-----------------|
| 1  | Seventh Wonder  |
| 2  | Metallica       |
| 3  | The Ocean       |
| 4  | Within Temptation |
| 5  | Death           |
| 6  | Van Canto       |
| 7  | Dream Theater   |
```

**Task 2: Select only the names of all bands**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| name            |
|-----------------|
| Seventh Wonder  |
| Metallica       |
| The Ocean       |
| Within Temptation |
| Death           |
| Van Canto       |
| Dream Theater   |
```

**Task 3: Select all albums released before 2000**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| id | name                      | release_year | band_id |
|----|---------------------------|-------------|---------|
| 4  | ...And Justice for All    | 1988        | 2       |
| 6  | Master of Puppets        | 1986        | 2       |
| 9  | Enter                    | 1997        | 4       |
| 12 | Individual Thought Patterns | 1993      | 5       |
| 13 | Human                    | 1991        | 5       |
```

### 2. Filtering and Sorting

**Task 4: Find all albums with no release year**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| id | name        | release_year | band_id |
|----|-------------|-------------|---------|
| 1  | The Great Escape | NULL    | 1      |
```

**Task 5: Find all bands that have "Th" in their name**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| id | name            |
|----|-----------------|
| 3  | The Ocean       |
| 4  | Within Temptation |
| 5  | Death           |
| 7  | Dream Theater   |
```

**Task 6: Order albums by release year (latest first) and name alphabetically**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| id | name              | release_year | band_id |
|----|-------------------|-------------|---------|
| 2  | Tiara            | 2018        | 1       |
| 7  | Resist           | 2018        | 4       |
| 14 | A Storm to Come   | 2006       | 6       |
| ... | ...             | ...         | ...     |
```

### 3. Joins and Relationships

**Task 7: List all albums with their band names**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| album_name                  | band_name       |
|-----------------------------|-----------------|
| The Great Escape           | Seventh Wonder  |
| Tiara                      | Seventh Wonder  |
| Mercy Falls                | Seventh Wonder  |
| Master of Puppets          | Metallica       |
| ...And Justice for All     | Metallica       |
| ...                        | ...             |
```

**Task 8: Find all bands that have no albums**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name      |
|----------------|
| Dream Theater  |
```

**Task 9: List all songs with their album and band names**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| song_name      | song_length | album_name           | band_name       |
|----------------|------------|----------------------|-----------------|
| The Great Escape | 30.23      | The Great Escape    | Seventh Wonder  |
| Welcome to Mercy Falls | 5.12 | Mercy Falls        | Seventh Wonder  |
| One              | 7.24      | ...And Justice for All | Metallica    |
| ...              | ...       | ...                  | ...            |
```

### 4. Aggregations and Grouping

**Task 10: Count the number of albums each band has**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name        | album_count |
|------------------|-------------|
| Seventh Wonder   | 3           |
| Metallica        | 3           |
| The Ocean        | 3           |
| Within Temptation| 3           |
| Death            | 3           |
| Van Canto        | 3           |
| Dream Theater    | 0           |
```

**Task 11: Find the average song length for each album**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| album_name            | average_length |
|-----------------------|----------------|
| The Great Escape      | 8.5            |
| Tiara                | 4.35           |
| ...And Justice for All | 6.42         |
| ...                   | ...           |
```

**Task 12: Find the number of songs for each band**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name        | song_count |
|------------------|------------|
| Seventh Wonder   | 35         |
| Metallica        | 27         |
| The Ocean        | 31         |
| Within Temptation| 30         |
| Death            | 27         |
| Van Canto        | 32         |
| Dream Theater    | 0          |
```

### 5. Data Modification

**Task 13: Insert a new band**
```sql
-- Solution placeholder
```

Expected Outcome:
```
Query OK, 1 row affected
```

**Task 14: Update album release year for an album with no release year**
```sql
-- Solution placeholder
```

Expected Outcome:
```
Query OK, 1 row affected
Rows matched: 1  Changed: 1  Warnings: 0
```

**Task 15: Delete a band that has no albums**
```sql
-- Solution placeholder
```

Expected Outcome:
```
Query OK, 1 row affected
```

### 6. Subqueries and Complex Queries

**Task 16: Find all bands that have albums released after 2015**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name        |
|------------------|
| Seventh Wonder   |
| Within Temptation|
```

**Task 17: Find albums that have songs longer than 8 minutes**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| album_name           | band_name       |
|----------------------|-----------------|
| The Great Escape     | Seventh Wonder  |
| Mercy Falls          | Seventh Wonder  |
| ...And Justice for All | Metallica     |
| ...                  | ...             |
```

**Task 18: Find bands that have more than 10 songs**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name        | song_count |
|------------------|------------|
| Seventh Wonder   | 35         |
| Metallica        | 27         |
| The Ocean        | 31         |
| Within Temptation| 30         |
| Death            | 27         |
| Van Canto        | 32         |
```

### 7. Advanced SQL Techniques

**Task 19: Find the longest song for each band**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name       | song_name        | song_length |
|-----------------|------------------|-------------|
| Seventh Wonder  | The Great Escape | 30.23       |
| Metallica       | ...And Justice for All | 9.82 |
| The Ocean       | Mesopelagic: Into the Uncanny | 9.28 |
| ...             | ...              | ...         |
```

**Task 20: Rank songs by length within each album**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| album_name      | song_name        | song_length | rank |
|-----------------|------------------|-------------|------|
| The Great Escape| The Great Escape | 30.23       | 1    |
| The Great Escape| Wiseman          | 5.42        | 2    |
| Mercy Falls     | Unbreakable      | 9.48        | 1    |
| Mercy Falls     | Welcome to Mercy Falls | 5.12  | 2    |
| ...             | ...              | ...         | ...  |
```

**Task 21: Create a view to show complete album information**
```sql
-- Solution placeholder
```

Expected Outcome:
```
| band_name       | album_name      | release_year | song_count | total_length |
|-----------------|-----------------|--------------|------------|--------------|
| Seventh Wonder  | The Great Escape| 2010         | 8          | 68.5         |
| Seventh Wonder  | Tiara          | 2018         | 13         | 56.6         |
| ...             | ...            | ...          | ...        | ...          |
```

### 8. Performance and Optimization

**Task 22: Create indexes to improve query performance**
```sql
-- Solution placeholder
```

Expected Outcome:
```
Query OK, 0 rows affected
Records: 0  Duplicates: 0  Warnings: 0
```

**Task 23: Create a stored procedure to get band statistics**
```sql
DELIMITER //
CREATE PROCEDURE GetBandStats(IN band_name_param VARCHAR(255))
BEGIN
    SELECT b.name AS band_name,
           COUNT(DISTINCT a.id) AS album_count,
           COUNT(s.id) AS song_count,
           AVG(s.length) AS avg_song_length,
           SUM(s.length) AS total_song_length
    FROM bands b
    LEFT JOIN albums a ON b.id = a.band_id
    LEFT JOIN songs s ON a.id = s.album_id
    WHERE b.name = band_name_param
    GROUP BY b.id, b.name;
END //
DELIMITER ;

-- Call example:
CALL GetBandStats('Metallica');

-- Result:
/*
| band_name | album_count | song_count | avg_song_length | total_song_length |
|-----------|-------------|------------|----------------|-------------------|
| Metallica | 3           | 27         | 6.58           | 177.6             | 
*/
```

**Task 24: Create a function to calculate album length**
```sql
DELIMITER //
CREATE FUNCTION AlbumLength(album_id_param INT) 
RETURNS FLOAT DETERMINISTIC
BEGIN
    DECLARE total_length FLOAT;
    
    SELECT SUM(length) INTO total_length
    FROM songs
    WHERE album_id = album_id_param;
    
    RETURN total_length;
END //
DELIMITER ;

-- Usage example:
SELECT name, AlbumLength(id) AS total_length FROM albums WHERE id = 1;

-- Result:
/*
| name            | total_length |
|-----------------|--------------|
| The Great Escape| 68.5         |
*/
```

## Contributing

Contributions to improve exercises or add new ones are welcome! Please submit a pull request.

## License

This project is available for educational purposes.
