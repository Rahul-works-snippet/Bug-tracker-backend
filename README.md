# 🚀 BugTracker API

A production-style backend for a Jira-inspired issue tracking system that enables teams to manage projects, track bugs, assign tickets, and collaborate efficiently.

Built with **Node.js, Express, MongoDB**, and **JWT authentication**, this API follows clean architecture principles and secure backend practices.

---

## 🔥 Live API

*(Add your Render URL here after deployment)*
Example:

```
https://bugtracker-api.onrender.com
```

---

## 🧠 Architecture Overview

```
Client (React / Vite)
        ↓
REST API (Express.js)
        ↓
Authentication Middleware (JWT)
        ↓
Business Logic (Controllers)
        ↓
MongoDB Atlas (Cloud Database)
```

This layered design improves scalability, security, and maintainability.

---

## ⚙️ Tech Stack

* **Node.js** — Runtime environment
* **Express.js** — Web framework for building REST APIs
* **MongoDB Atlas** — Cloud-hosted NoSQL database
* **Mongoose** — ODM for schema modeling
* **JWT** — Secure authentication
* **bcrypt** — Password hashing
* **dotenv** — Environment configuration
* **CORS** — Cross-origin requests

---

## ✨ Core Features

✅ User Authentication (Register / Login)
✅ Encrypted Password Storage
✅ JWT-based Route Protection
✅ Project Creation & Management
✅ Ticket / Issue Tracking
✅ Ticket Assignment
✅ Status Workflow (To Do → In Progress → Done)
✅ Priority Levels
✅ Protected Routes
✅ Scalable Folder Structure

---

## 📁 Folder Structure

```
backend/
│
├── config/        # Database connection
├── controllers/  # Route logic
├── middleware/   # Auth & error handling
├── models/       # Mongoose schemas
├── routes/       # API routes
├── .env          # Environment variables (ignored)
├── .gitignore
├── package.json
└── server.js
```

---

## 🔐 Environment Variables

Create a `.env` file in the root:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_super_secret_key
PORT=5000
```

⚠️ Never commit `.env` to GitHub.

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository

```
git clone https://github.com/YOUR_USERNAME/bugtracker-api.git
```

### 2️⃣ Navigate into the project

```
cd bugtracker-api
```

### 3️⃣ Install dependencies

```
npm install
```

### 4️⃣ Start the server

```
npm run dev
```

or

```
node server.js
```

Server runs on:

```
http://localhost:5000
```

---

## 🔑 API Endpoints (Example)

### Auth

```
POST /api/users/register
POST /api/users/login
```

### Projects

```
POST /api/projects
GET /api/projects
```

### Tickets

```
POST /api/tickets
GET /api/tickets
PATCH /api/tickets/:id
DELETE /api/tickets/:id
```

---

## 🧪 Health Check

```
GET /
```

Response:

```
BugTracker API Live
```

Useful for deployment verification.

---

## 🚀 Deployment

This API is optimized for cloud deployment.

**Recommended stack:**

* Render — Backend hosting
* MongoDB Atlas — Database

After deployment, remember to add environment variables inside Render.

---

## 🔒 Security Practices

* Passwords hashed with bcrypt
* JWT authentication
* Protected routes
* Environment-based secrets
* Gitignored sensitive files

---

## 🎯 Future Enhancements

* Role-based access control
* File attachments for tickets
* Real-time updates with Socket.io
* Activity logs
* Email notifications
* Advanced filtering & search

---

## 👨‍💻 Author

**Rahul Mallick**

If you found this project useful or inspiring, feel free to connect!

---

## ⭐ Why This Project Matters

This is not just a CRUD demo — it is designed to reflect how modern teams build workflow software, emphasizing:

* Clean backend architecture
* Secure authentication
* Real-world data relationships
* Scalable structure

---

💡 *Built to simulate production-grade backend engineering.*
