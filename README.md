# Backend Assignment

This project contains two backend REST APIs developed using Node.js, Express.js, MongoDB Atlas, and Mongoose.

---

# 📌 Technologies Used

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- bcryptjs
- dotenv
- nodemon

---

# 📘 Task 1: Student API (Port 5000)

## 📂 Run Project

```bash
cd Task1_StudentAPI
npm install
npm run dev
```

---

## 🔐 .env File

Create a `.env` file inside `Task1_StudentAPI` folder:

```env
PORT=5000
MONGODB_URI=mongodb+srv://786ghulamdastageer_db_user:codewithmongo%402026@devtaminapi.ya8h86a.mongodb.net/student_management?appName=DevtaminAPI
```

---

## 📌 Student API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/students` | Create new student |
| GET | `/api/students` | Get all students |
| GET | `/api/students/:id` | Get student by ID |
| GET | `/api/students/search?name=` | Search student by name |
| PUT | `/api/students/:id` | Update complete student |
| PATCH | `/api/students/:id` | Partial update student |
| DELETE | `/api/students/:id` | Delete student |
| PATCH | `/api/students/:id/deactivate` | Deactivate student |

---

## 📌 Features

- Complete CRUD Operations
- Search Students by Name
- Student Deactivation
- MongoDB Atlas Integration
- RESTful API Structure
- Error Handling

---

# 📘 Task 2: Blog Application API (Port 5001)

## 📂 Run Project

```bash
cd Task2_BlogAPI
npm install
npm run dev
```

---

## 🔐 .env File

Create a `.env` file inside `Task2_BlogAPI` folder:

```env
PORT=5001
MONGODB_URI=mongodb+srv://786ghulamdastageer_db_user:codewithmongo%402026@devtaminapi.ya8h86a.mongodb.net/blog_platform?appName=DevtaminAPI
BCRYPT_ROUNDS=10
```

---

# 📌 User Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/users/register` | Register new user |
| GET | `/api/users` | Get all users |
| GET | `/api/users/:id` | Get user by ID |

---

# 📌 Post Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/posts` | Create new post |
| GET | `/api/posts` | Get all posts |
| GET | `/api/posts/:id` | Get post by ID |
| GET | `/api/posts/tag/:tag` | Get posts by tag |
| PUT | `/api/posts/:id` | Update post |
| DELETE | `/api/posts/:id` | Delete post |

---

# 📌 Comment Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/posts/:postId/comments` | Add comment |
| GET | `/api/posts/:postId/comments` | Get all comments |
| DELETE | `/api/comments/:id` | Delete comment |

---

# 📌 Features

- User Registration
- Blog Post Management
- Comment System
- Tag Filtering
- Password Hashing using bcrypt
- RESTful API Architecture
- MongoDB Atlas Integration

---

# ▶️ Run Both Servers Together

## Terminal 1

```bash
cd Task1_StudentAPI
npm run dev
```

## Terminal 2

```bash
cd Task2_BlogAPI
npm run dev
```

---

# 🧪 API Testing

You can test APIs using:

- Postman
- Thunder Client
- Insomnia

---

# 📌 Example Base URLs

```bash
http://localhost:5000/api/students

http://localhost:5001/api/posts
```

---

# 👨‍💻 Author

## Ghulam Dastageer

- BS Computer Science Student
- FAST NUCES

GitHub: github.com/786ghulamdastageer

---

# ⭐ Notes

- Make sure MongoDB Atlas connection is working.
- Install dependencies before running servers.
- Use separate terminals for both APIs.
- Nodemon automatically restarts server during development.
