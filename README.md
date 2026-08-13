Todo Management System

A simple Todo Management System built with Java and Spring Boot. The application allows users to manage tasks using CRUD operations, with task data stored in a MySQL database.

Features

Add new tasks

View all tasks

Update task details

Mark tasks as completed

Delete tasks

Persistent task storage using MySQL

Tech Stack

Java

Spring Boot

Spring Web

Spring Data JPA

MySQL

Thymeleaf

Lombok

Maven

Project Architecture

The application follows a layered architecture:

Browser
   ↓
Controller
   ↓
Service
   ↓
Repository
   ↓
Spring Data JPA / Hibernate
   ↓
MySQL

Layers

Controller: Handles incoming HTTP requests and returns responses/views.

Service: Contains the application's business logic.

Repository: Handles database operations using Spring Data JPA.

Entity/Model: Represents the task data stored in the database.

Thymeleaf: Used for rendering the web pages on the server side.

CRUD Operations

The application implements the following operations:

Operation

Description

Create

Add a new task

Read

View existing tasks

Update

Modify task details / completion status

Delete

Remove a task

Database

The application uses MySQL for persistent data storage and Spring Data JPA for database interaction.

Configure your MySQL database connection in the application's configuration file before running the project.

Example:

spring.datasource.url=jdbc:mysql://localhost:3306/your_database
spring.datasource.username=your_username
spring.datasource.password=your_password

Do not commit real database passwords or other sensitive credentials to GitHub.

Getting Started

Prerequisites

Make sure you have installed:

Java JDK

Maven

MySQL

Git

Run the Project

Clone the repository:

git clone <your-github-repository-url>

Open the project in your IDE.

Create a MySQL database.

Configure the database credentials in the application's configuration file.

Build and run the Spring Boot application:

mvn spring-boot:run

Open the application in your browser using the configured local port.

What I Learned

Through this project, I practiced:

Building a web application with Spring Boot

Creating CRUD functionality

Using Spring Data JPA repositories

Connecting a Spring Boot application with MySQL

Working with Entity, Controller, Service, and Repository layers

Using Thymeleaf for server-side page rendering

Using Lombok to reduce boilerplate code

Future Improvements

Possible future improvements include:

User authentication and authorization

Task categories and priorities

Due dates and reminders

Search and filtering

REST API endpoints

Responsive UI improvements

Author

Rohit Kumar

GitHub: https://github.com/rohitkumar2702

LinkedIn: https://www.linkedin.com/in/rohit-kumar-611456306
