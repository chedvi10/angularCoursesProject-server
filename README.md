# Angular Project Server 2

This is the backend server for the Angular Project 2. It provides API endpoints for managing courses, users, categories, and lecturers.

## Features

- User authentication (login and registration)
- Course management (list, add, update)
- Category and lecturer information
- Lecturer verification

## Technologies Used

- Node.js
- Express.js
- File-based JSON storage

## Setup

1. Install dependencies:
2. Start the server:

The server will run on port 3000 by default.

## API Endpoints

### Courses
- GET `/api/courses`: Get all courses
- GET `/api/courses/:id`: Get a specific course
- POST `/api/add-course`: Add a new course
- PUT `/api/courses/:id`: Update a course

### Categories
- GET `/api/categories`: Get all categories

### Lecturers
- GET `/api/lecturers`: Get all lecturers

### Users
- GET `/api/users/:id`: Get a specific user

### Authentication
- POST `/api/login`: User login
- POST `/api/register`: User registration
- POST `/api/verify-lecturer-code`: Verify lecturer code

## Data Storage

The application uses JSON files to store data:
- `users.json`: Store user information
- `courses.json`: Store course information
- `categories.json`: Store category information
- `lecturers.json`: Store lecturer information

## Notes

- The server uses CORS to allow cross-origin requests.
- Passwords are stored in plain text. In a production environment, implement proper password hashing.
- The lecturer verification code is hardcoded. Replace with a secure method in production.


