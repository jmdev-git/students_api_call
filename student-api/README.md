# Student API

Name: GRADO, MARY

Project Title: API-CALL

This project demonstrates a RESTful API built with Laravel 11 that handles student record management. It supports full CRUD operations through structured API endpoints and returns JSON responses. All endpoints were tested and verified using Postman.

---

## How to Run

1. Open the project folder in VS Code
2. Open the terminal and run: `php artisan serve`
3. Launch Postman for API testing
4. Test the following HTTP methods: GET, POST, PUT, PATCH, DELETE
5. Use the base endpoint: `http://127.0.0.1:8000/api/students`
6. Check the JSON responses returned from the database

---

## Endpoints Overview

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/students` | Retrieve all students |
| GET | `/api/students/{id}` | Retrieve a specific student |
| POST | `/api/students` | Add a new student |
| PUT | `/api/students/{id}` | Replace all fields of a student |
| PATCH | `/api/students/{id}` | Update specific fields only |
| DELETE | `/api/students/{id}` | Remove a specific student |
| DELETE | `/api/students` | Remove all students |

---

## Screen Recording Demonstration

[View Demo Here](YOUR_VIDEO_LINK_HERE)
