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

![Screenshot 2024-06-14 111852](https://github.com/Tejas-24ytj/Employee-Management-System/assets/105742352/41723e7c-3ae7-4647-a414-8106a3666ec3)
![Screenshot 2024-06-14 111733](https://github.com/Tejas-24ytj/Employee-Management-System/assets/105742352/b4d22721-e826-4103-a862-bdc65b2e477c)
![Screenshot 2024-06-14 111719](https://github.com/Tejas-24ytj/Employee-Management-System/assets/105742352/6f1c6e33-9591-4cff-b0f4-3004b67da93b)
![Screenshot 2024-06-14 111543](https://github.com/Tejas-24ytj/Employee-Management-System/assets/105742352/95bddd01-4ad6-4df1-bc53-98e11c49c63c)

