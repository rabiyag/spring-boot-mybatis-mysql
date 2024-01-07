# Spring Boot MyBatis MySQL

This project demonstrates integrating MyBatis with Spring Boot to manage MySQL database interactions, offering a flexible, SQL-mapping-based persistence layer.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Running the Application](#running-the-application)
- [Usage](#usage)

## Features
- MyBatis Integration: Simplifies SQL mapping and CRUD operations.
- Spring Boot Configuration: Easy setup and configuration of MyBatis.
- MySQL Support: Connects and manages data using MySQL.
- Repository Layer: Clean separation of database logic.
- Environment Management: Uses properties for configuring MySQL connection.

## Technologies Used
- **Spring Boot** (backend framework)
- **MySQL** (database)
- **MyBatis Spring Boot Starter** 
- **Maven** (dependency management)

## Prerequisites
- **JDK 8** or higher
- **Maven** for dependency management
- **PostgreSQL** database

## Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/rabiyag/spring-boot-mybatis-mysql.git
    cd spring-boot-mybatis-mysql
   ```

2. **Update application.properties with your database connection details:**:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/your_database
    spring.datasource.username=your_db_username
    spring.datasource.password=your_db_password
    ```
   
3. **Build the project with Maven**:
   ```bash
   mvn clean install
   ```

## Running the Application
1. **Run the application**:
   ```bash
   mvn spring-boot:run
   ```

2. **Access the application**:
   - The application will be available at http://localhost:8080:
  

## Usage
This application serves as a foundational example for using MyBatis with Spring Boot to manage CRUD operations in a MySQL database. Here’s how it can be utilized:

1. Define Mappers: Write SQL queries directly in XML mapper files or annotate methods in Java interfaces to perform CRUD operations.

2. Create API Endpoints: Build RESTful endpoints in the controller layer to interact with the MyBatis mappers. This can include endpoints for creating, reading, updating, and deleting records in the MySQL database.

3. Execute Queries: MyBatis will map Java objects to SQL queries, enabling seamless interaction with the database. The application can be customized to perform specific queries based on business requirements.

4. Error Handling and Transactions: Use Spring Boot’s support for transactions and exception handling to ensure data integrity.

This setup is ideal for applications requiring fine-grained control over SQL queries without writing extensive boilerplate code. You can extend it by adding more complex queries or integrating additional MyBatis features like dynamic SQL.
