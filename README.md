# Employee Management System

This is a simple Employee Management System built with Java Spring Boot, Thymeleaf for the frontend, and MySQL RDS for the database. It allows you to create, update, delete, and retrieve employee records.

## Features

- Add new employees
- View a list of all employees
- Update employee information
- Delete employees

## Technologies Used

- Java Spring Boot
- Thymeleaf
- MySQL RDS
- Maven

## Prerequisites

- Java 11 or higher
- Maven
- MySQL database

## Getting Started

### Clone the Repository

```sh
git clone https://github.com/yourusername/employee-management-system.git
cd employee-management-system

spring.datasource.url=jdbc:mysql://${DB_HOST}:${DB_PORT}/${DB_NAME}
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect

### Generation of Jar
mvn clean package
java -jar target/employee-management-system-0.0.1-SNAPSHOT.jar

### Deployment on elastic beanstalk
eb init -p java-11 employee-management-system --region your-region
eb create employee-management-env
eb deploy
eb setenv DB_HOST=your-database-host DB_PORT=your-database-port DB_NAME=your-database-name DB_USER=your-database-username DB_PASSWORD=your-database-password


## Images


![Screenshot 2024-06-14 111852](https://github.com/Tejas-24ytj/Employee-Management-System/assets/105742352/359c6bd7-4d1a-4869-8767-ad38955d2aeb)

