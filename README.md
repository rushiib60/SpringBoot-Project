# Spring Boot Student Management System

A full-stack CRUD application for managing student records, built with a Spring Boot REST API backend and Angular frontend.

## Features

- Add, view, update, and delete student records
- RESTful API with Spring Boot
- Responsive Angular frontend with forms and data tables
- In-memory H2 database (easy to swap for MySQL/PostgreSQL)

## Project Structure

```
SpringBootApplication/    # Backend — Spring Boot (Java)
│   ├── src/
│   │   ├── main/java/    # Controllers, Services, Models, Repositories
│   │   └── resources/    # application.properties
│   └── pom.xml
│
student-form-angular/     # Frontend — Angular
    ├── src/
    │   └── app/          # Components, services
    └── package.json
```

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Java, Spring Boot, Spring Data JPA |
| Frontend | Angular, TypeScript |
| Database | H2 (in-memory) / MySQL |
| Build | Maven |

## Getting Started

### Prerequisites

- Java 11+
- Maven
- Node.js + Angular CLI (`npm install -g @angular/cli`)

### Backend

```bash
cd SpringBootApplication
mvn spring-boot:run
```

API runs at `http://localhost:8080`

### Frontend

```bash
cd student-form-angular
npm install
ng serve
```

Open `http://localhost:4200` in your browser.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get student by ID |
| POST | `/api/students` | Add new student |
| PUT | `/api/students/{id}` | Update student |
| DELETE | `/api/students/{id}` | Delete student |
