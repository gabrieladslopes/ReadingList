# ReadingList Project

Reading List is a project proposed in the book "Spring Boot in Action".

I've used this project to learn how to develop a Spring application using Spring Boot. The starter dependencies chosen for this development were: Spring Web, Spring Data JPA, Thymeleaf, H2 Database and the development dependency Spring Boot Devtools. Also, the build tool used was Maven. 

The Spring Secutiry dependency was added as an example of how to add a starter dependency and override an auto-configuration afterwards.

# Application

## Book Entity

The Book entity represents a book and reflects a table in the database.

Annotations:
* @Entity - specifies that the class is an entity
* @Id - specifies the primary key of a table
* @GeneratedValue - indicates that the value will be automatically provided

## ReadingList Repository

Repository through which the ReadingList objects will be persisted to the database. Since we're using the Spring Data JPA we create an interface that extends the JpaRepository interface.

## ReadingList Controller

A Spring MVC controller which handles HTTP requests for the application.

Annotations:
* @Controller - anotates this controller in order to be picked up by component-scanning and automatically be registered as a bean in the Spring application context
* @RequestMapping - maps all handler methods to a base URL path of "/readingList" 

## ReadingList View

A Thymeleaf template that presents a reading list: readingList.html

## SecurityConfig

A class used to explicitly define some security configuration in order to override spring-starter-security auto-configuration.

The users are going to be authenticated against the database via JPA.

Annotation:
* @Configuration - 
* @EnableWebSecurity - 


## Reader Repository

Spring Data JPA repository interface for persisting readers.


## Reader Entity

JPA entity with fields to capture the username, password and full name of the user.















