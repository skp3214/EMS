

# Employee Management System (EMS)

## Overview

The Employee Management System (EMS) is a web application that allows organizations to manage their employee data efficiently. It provides functionalities to create, read, update, and delete employee records. The application is built using Angular for the frontend and Spring Boot for the backend, with MySQL as the database.

https://github.com/user-attachments/assets/74857454-a55b-4a73-aa72-cf4a4274ce89

![image](https://github.com/user-attachments/assets/c4dbd0e5-c3e8-42b2-8b8a-6f78658f6bb6)

## Features

- **Employee List**: View a list of all employees.
- **Add Employee**: Add new employee records.
- **Edit Employee**: Update existing employee records.
- **Delete Employee**: Remove employee records.
- **View Employee Details**: View details of a specific employee.

## Technologies Used

### Frontend

- Angular
- HTML
- CSS
- TypeScript
- Angular Material

### Backend

- Spring Boot
- Spring Data JPA
- MySQL

### Tools

- Visual Studio Code
- Postman
- MySQL Workbench

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Java 11 or later installed
- Node.js and npm installed
- Angular CLI installed
- MySQL installed and running

## Setup Instructions

### Backend Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/skp3214/ems.git
    cd backend
    ```

2. Update the MySQL configuration in `application.properties`:

    ```properties
    server.port=8080
    spring.datasource.url=jdbc:mysql://<YOUR_MYSQL_HOST>:<YOUR_MYSQL_PORT>/defaultdb?useSSL=false
    spring.datasource.username=<USERNAME>
    spring.datasource.password=<YOUR_PASSWORD>
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.jpa.hibernate.ddl-auto=update
    ```

3. Run the Spring Boot application:

    ```bash
    ./mvnw spring-boot:run
    ```

### Frontend Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/skp3214/ems.git
    cd frontend
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Start the Angular application:

    ```bash
    ng serve
    ```

    The application will be available at `http://localhost:4200`.


## API Endpoints

The backend exposes the following API endpoints:

- `GET /api/v1/employees` - Retrieve all employees
- `POST /api/v1/employees` - Create a new employee
- `GET /api/v1/employees/{id}` - Retrieve an employee by ID
- `PUT /api/v1/employees/{id}` - Update an employee by ID
- `DELETE /api/v1/employees/{id}` - Delete an employee by ID

- Thanks to the creators of Angular, Spring Boot, and MySQL for their amazing tools and frameworks.

---

