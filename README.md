# ReadingList Project

Reading List project learned in the Spring Boot in Action book.

I've used this project to learn how to develop a Spring application using Spring Boot. The dependencies chosen for this development were: Spring Web, Spring Data JPA, Thymeleaf, H2 Database and the development dependency Spring Boot Devtools. The build tool used was Maven. 

# Application

## Book Entity

The Book entity represents a book and will represent a table in the database.

Annotations:
* @Entity - specifies that the class in an entity
* @Id - specifies the primary key of a table
* @GeneratedValue - indicates that the value will be automatically provided

## ReadingList Repository

Repository through which the ReadingList objects will be persisted to the database. Since we're using the Spring Data JPA we create an interface that extends the JpaRepository interface.

## ReadingList Controller

A Spring MVC controller which will handle HTTP requests for the application.

Annotations:
* @Controller - anotates this controller in order for it to be picked up by component-scanning and automatically be registered as a bean in the Spring application content
* @RequestMapping - map all handler methods to a base URL path of "/readingList" 

## ReadingList View

A Thymeleaf template that presents a reading list: readingList.html

