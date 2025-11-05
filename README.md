# ⚙️ TaskNest Backend

The **TaskNest Backend** provides secure RESTful APIs for user authentication and task management.  
Built with **Node.js**, **Express**, and **MongoDB**, it powers the frontend with robust and scalable endpoints.

---

## 🚀 Features

### 🔐 Authentication
- Register and Login endpoints  
- Secure password hashing using **bcrypt**  
- **JWT-based authentication** for protected routes  

### ✅ Task Management
- Add, Edit, Delete, and View user-specific tasks  
- Each task includes:
  - 🏷️ Title  
  - 📄 Description  
  - 📆 Due Date  
  - ⚡ Priority Level  
  - ✅ Completion Status  

---

## 🧱 Technologies Used

| Category | Technology |
|-----------|-------------|
| Runtime | Node.js |
| Framework | Express.js |
| Database | MongoDB + Mongoose |
| Authentication | JWT (JSON Web Token) |
| Password Hashing | bcrypt |
| Environment Config | dotenv |
| Middleware | CORS, express.json(), custom auth middleware |

---

## 🧩 API Endpoints

### 👤 User Routes
| Method | Endpoint | Description |
|--------|-----------|-------------|
| POST | `/api/register` | Register a new user |
| POST | `/api/login` | Log in existing user |

### 📋 Task Routes
| Method | Endpoint | Description |
|--------|-----------|-------------|
| GET | `/api/tasks` | Fetch all tasks for the logged-in user |
| POST | `/api/tasks` | Add a new task |
| PUT | `/api/tasks/:id` | Update a specific task |
| DELETE | `/api/tasks/:id` | Delete a specific task |

---

## 🧩 Models

### 🧑 User Model
| Field | Type | Description |
|-------|------|-------------|
| `name` | String | Full name of the user |
| `email` | String | Unique email address |
| `password` | String | Hashed password |

### 🗂️ Task Model
| Field | Type | Description |
|-------|------|-------------|
| `title` | String | Title of the task |
| `description` | String | Description of the task |
| `dueDate` | Date | Deadline for the task |
| `priority` | String | Low, Medium, or High |
| `completed` | Boolean | Task completion status |
| `user` | ObjectId | Reference to the user |

---

## 🔒 Middleware
- **Authentication Middleware** — Verifies JWT and authorizes user  
- **CORS Middleware** — Enables frontend-backend communication  

---

## 🔐 Security
- Passwords hashed using **bcrypt**  
- JWT tokens stored securely  
- Protected routes require valid token  
- Validation on both frontend and backend  

---

## 🌟 Highlights
- Full CRUD APIs for tasks  
- Secure authentication  
- Modular and scalable structure  
- Follows MVC pattern  
- Beginner-friendly and clean codebase  

---

## 👩‍💻 Author
**Sanjana A K**  
📧 [sanjanaak556@gmail.com]
