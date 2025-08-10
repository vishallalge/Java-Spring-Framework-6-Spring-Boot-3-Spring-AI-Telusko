
# Hibernate :


## What is Hibernate? 
- Hibernate is an Object-Relational Mapping (ORM) framework for Java. 
- It helps developers interact with a relational database (like MySQL, PostgreSQL, etc.) using Java objects, without having to write complex SQL queries manually.


## Project Setup - 
- Get all the dependencies from MVN repository.
- Link - 
    `https://mvnrepository.com/artifact/com.mysql/mysql-connector-j/9.1.0`


## Lazy Fetching - (Default in Hibernate)
- Related data is not loaded immediately when you fetch the parent entity.

- Instead, Hibernate loads the related data only when you actually access it (on-demand).

## Eager Fetching -
- Related data is loaded immediately along with the parent entity, in the same query via `JOIN` or through multiple queries.


## What is Caching?
- Caching is the process of storing frequently used data in memory so it can be accessed faster later, instead of repeatedly fetching it from a slower source like a database or disk.


## What is HQL?
- HQL (Hibernate Query Language) is Hibernate’s object-oriented query language used to fetch, update, or delete data from a database.

-  Difference between SQL and HQL :

        SQL: SELECT * FROM employee WHERE salary > 50000;

        HQL: FROM Employee e WHERE e.salary > 50000
