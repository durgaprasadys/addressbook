# Contact Management System

A full-stack contact management application built with React, Spring Boot, and MySQL.

## Features

- Create, read, update, and delete contacts
- Search contacts by name, email, or phone
- Responsive design with Tailwind CSS
- RESTful API backend
- MySQL database integration

## Prerequisites

- Node.js (v14 or higher)
- Java 17 or higher
- MySQL 8.0 or higher
- Maven

## Setup

### Database Setup

1. Create a MySQL database:
```sql
CREATE DATABASE addressbook;
```

2. Update the database configuration in `backend/src/main/resources/application.properties` with your MySQL credentials.

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Build the project:
```bash
mvn clean package
```

3. Run the application:
```bash
java -jar target/addressbook-1.0-SNAPSHOT.jar
```

The backend will run on http://localhost:8080

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The frontend will run on http://localhost:3000

## Production Build

### Frontend Build
```bash
cd frontend
npm run build
```

### Backend Build
```bash
cd backend
mvn clean package
```

The production build will be available in `backend/target/addressbook-1.0-SNAPSHOT.jar`

## API Endpoints

- GET /api/contacts - Get all contacts
- GET /api/contacts/{id} - Get contact by ID
- POST /api/contacts - Create new contact
- PUT /api/contacts/{id} - Update contact
- DELETE /api/contacts/{id} - Delete contact

## Technologies Used

- Frontend:
  - React
  - Tailwind CSS
  - Axios
  - React Router

- Backend:
  - Spring Boot
  - Spring Data JPA
  - MySQL
  - Lombok

## License

MIT 