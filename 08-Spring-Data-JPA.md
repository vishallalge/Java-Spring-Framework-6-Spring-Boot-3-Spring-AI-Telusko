
# Spring Data JPA :


## What is JPA? 

- JPA (`Java Persistence API`) is a specification in Java that defines how to manage relational data (`databases`) using Java objects.
- It’s a specification in Java that defines how to work with relational databases using objects. 
- It is not an implementation itself, but frameworks like Hibernate implement JPA. 
- In Spring Boot, we use Spring Data JPA which internally uses Hibernate to simplify database operations.


## What is ORM and JPA :

- ORM is a concept of mapping objects to relational tables. 
- JPA is a Java specification that standardizes ORM in Java. 
- JPA doesn’t do ORM itself; instead, frameworks like Hibernate implement JPA to perform ORM
| **Aspect**         | **ORM** (Object Relational Mapping)                                           | **JPA** (Java Persistence API)                                               |
| ------------------ | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **Definition**     | A **concept/technique** of mapping Java objects to relational database tables | A **specification (standard)** in Java that defines how ORM should be done   |
| **Scope**          | General approach used in many languages (Java, Python, etc.)                  | Specific to Java ecosystem                                                   |
| **What it is**     | A **methodology** (not tied to Java)                                          | A **Java API specification**                                                 |
| **Implementation** | Implemented by frameworks like Hibernate, EclipseLink, etc.                   | Implemented by ORM frameworks (Hibernate, EclipseLink, OpenJPA, etc.)        |
| **Usage**          | Just a concept, doesn’t provide direct API                                    | Provides a standard API with annotations (`@Entity`, `@Id`, etc.)            |
| **Example**        | ORM → concept of mapping `User` class → `users` table                         | JPA → defines standard annotations & interfaces (`EntityManager`, `@Entity`) |
