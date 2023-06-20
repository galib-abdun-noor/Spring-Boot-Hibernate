# What is JPA?
JPA stands for Java Persistence API.
- It is a specification in Java EE for object-relational mapping (ORM).
- JPA bridges the gap between object-oriented programming and relational databases.
- It allows developers to map Java objects to database tables.
- JPA provides a set of APIs for managing relational data.
- It eliminates the need for developers to write complex SQL queries.
- JPA includes concepts like entities (Java classes representing database tables) and relationships between entities.
- It also provides a query language called JPQL (Java Persistence Query Language) for executing queries against the mapped entities.

# What are Benefits of JPA?
- Object-Relational Mapping (ORM): JPA provides an abstraction layer that maps Java objects to relational database tables, allowing developers to work with objects instead of writing raw SQL queries.
- Database Independence: JPA supports multiple database vendors, allowing applications to be easily switched between different databases without significant code changes.
- Simplified Data Access: JPA provides a high-level API for performing database operations, eliminating the need to write boilerplate JDBC code. It handles tasks such as connection management, transaction handling, and caching automatically.

# What is Hibernate?
Hibernate is an open-source ORM (Object-Relational Mapping) framework for Java. In Spring Boot, Hibernate is the default implementation of JPA
- It simplifies database interactions by mapping Java objects to database tables.
- Developers can define persistent classes (entities) that represent database tables.
- Hibernate handles CRUD operations (Create, Read, Update, Delete) using object-oriented methods.
- It abstracts away low-level database details, such as SQL queries and connection management.

# CRUD Apps
- ## Create (Insert): 
    To create a new record in the database, you create a new instance of the entity class, set its properties, and persist it using the     EntityManager (provided by JPA). The EntityManager ensures that the entity is inserted into the database.
- ## Read (Retrieve):
    To retrieve records from the database, you use queries or find methods provided by JPA. You can retrieve entities based on their        primary keys or perform more complex queries using JPQL (Java Persistence Query Language) or Criteria API.
- ## Update: 
    To update an existing record, you retrieve the entity from the database, modify its properties, and commit the changes using the        EntityManager. The EntityManager tracks the changes and updates the corresponding record in the database when you commit the 
    transaction.
- ## Delete: 
    To delete a record, you retrieve the entity from the database using its primary key or a query, and then remove it using the            EntityManager. The EntityManager ensures that the corresponding record is deleted from the database.

# Spring Boot - Auto configuration
Spring Boot Auto-configuration is a feature provided by the Spring Boot framework.
- Spring Boot auto-configuration automatically configures the Spring application based on the jar dependencies that we have added.
- Auto-configuration works by scanning the classpath for specific libraries and components commonly used in Spring applications.
- When an auto-configuration class is found, Spring Boot automatically configures relevant beans and properties based on the detected dependencies.
- We can enable the auto-configuration feature by using the annotation @EnableAutoConfiguration. But this annotation does not use because it is wrapped inside the @SpringBootApplication annotation. The annotation @SpringBootApplication is the combination of three annotations: @ComponentScan, @EnableAutoConfiguration, and @Configuration.
### @SpringBootApplication=@ComponentScan+@EnableAutoConfiguration+@Configuration
