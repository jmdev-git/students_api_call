# Student API

A simple RESTful API built with **Laravel 11** for managing student records.

## 📹 Demo Video

[Click here to watch the Postman demo](YOUR_VIDEO_LINK_HERE)

---

## Tech Stack

- PHP 8.2
- Laravel 11
- SQLite
- Postman (for testing)

---

## Setup

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

Server runs at `http://127.0.0.1:8000`

---

## API Endpoints

Base URL: `http://127.0.0.1:8000/api`

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/students` | Get all students |
| GET | `/students/{id}` | Get a single student |
| POST | `/students` | Create a new student |
| PUT | `/students/{id}` | Full update of a student |
| PATCH | `/students/{id}` | Partial update of a student |
| DELETE | `/students/{id}` | Delete a student |
| DELETE | `/students` | Delete all students |

---

## Request Body

For `POST` and `PUT`, all fields are required:

```json
{
    "name": "Alice Reyes",
    "email": "alice@example.com",
    "course": "Computer Science"
}
```

For `PATCH`, only send the fields you want to update:

```json
{
    "course": "Data Science"
}
```

---

## Sample Responses

**POST /api/students** — `201 Created`
```json
{
    "id": 1,
    "name": "Alice Reyes",
    "email": "alice@example.com",
    "course": "Computer Science",
    "created_at": "2026-05-29T00:00:00.000000Z",
    "updated_at": "2026-05-29T00:00:00.000000Z"
}
```

**GET /api/students/{id}** — `404 Not Found`
```json
{
    "message": "Student not found!"
}
```
