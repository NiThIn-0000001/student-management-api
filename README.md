# Student Management System

A REST API built using Java Spring Boot and MySQL to manage student records.

## Technologies Used
- Java 21
- Spring Boot
- Spring Data JPA
- MySQL
- Maven
- Postman
- Newman

## Features
- Add a student
- View all students
- View a student by ID
- Update student details
- Delete a student

## Database Configuration
Configure these environment variables before running the application:
- DB_USERNAME
- DB_PASSWORD

Database name: `studentdb`

## Run the Application
```bash
./mvnw spring-boot:run
```

The API runs at: http://localhost:8080

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/students | Add student |
| GET | /api/students | Get all students |
| GET | /api/students/{id} | Get student by ID |
| PUT | /api/students/{id} | Update student |
| DELETE | /api/students/{id} | Delete student |

## API Testing
Import `Student_API_Collection.json` into Postman.

Run automated tests:
```bash
newman run Student_API_Collection.json
```

An HTML test report can be generated using Newman.
