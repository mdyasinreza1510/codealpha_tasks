# 🎟️ Event Registration System

A backend application built using **Node.js**, **Express.js**, and **MongoDB** for managing event registrations. The project provides REST APIs for user authentication, event management, and event registration using the MVC architecture.

---

# 🚀 Features

- User Registration
- User Login
- Password Hashing using BCrypt
- JWT Authentication
- Create Events
- View All Events
- View Event Details
- Register for an Event
- View My Registrations
- Cancel Registration

---

# 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- BCrypt
- JSON Web Token (JWT)
- Dotenv
- Postman

---

# 📂 Project Structure

```text
EVENT-REGISTRATION-SYSTEM
│
├── src
│   ├── controllers
│   │      auth.controller.js
│   │      event.controller.js
│   │      registration.controller.js
│   │
│   ├── db
│   │      db.js
│   │
│   ├── models
│   │      user.model.js
│   │      event.model.js
│   │      registration.model.js
│   │
│   ├── routes
│   │      auth.routes.js
│   │      event.routes.js
│   │      registration.routes.js
│   │
│   └── app.js
│
├── server.js
├── .env
├── .gitignore
├── package.json
└── README.md
```

---

# 🗄️ Database Models

## User

| Field | Type |
|------|------|
| name | String |
| email | String |
| password | String |

---

## Event

| Field | Type |
|------|------|
| title | String |
| description | String |
| date | Date |
| location | String |
| capacity | Number |
| organizer | ObjectId |

---

## Registration

| Field | Type |
|------|------|
| user | ObjectId |
| event | ObjectId |

---

# 📡 API Endpoints

## Authentication

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login user |

---

## Events

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/event/create` | Create a new event |
| GET | `/api/event` | View all events |
| GET | `/api/event/:id` | View event details |

---

## Registrations

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/register/:eventId` | Register for an event |
| GET | `/api/register/my` | View my registrations |
| DELETE | `/api/register/:registrationId` | Cancel a registration |

---

# 🔐 Authentication

JWT authentication is used for protected routes.

Users receive a JWT token after a successful login, which is sent in the Authorization header for authenticated requests.

---



---

# 🧪 API Testing

All APIs were tested using **Postman**.

---

# 👨‍💻 Author

**Md Yasin Reza**

---
