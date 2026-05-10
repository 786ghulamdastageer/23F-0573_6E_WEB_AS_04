MERN Backend Assignment APIs

A complete backend assignment containing two REST APIs built with Node.js, Express.js, MongoDB Atlas, and Mongoose.

📌 Project Structure
Backend-Assignment/
│
├── Task1_StudentAPI/
│
└── Task2_BlogAPI/
🚀 Technologies Used
Node.js
Express.js
MongoDB Atlas
Mongoose
bcryptjs
dotenv
nodemon
⚙️ MongoDB Atlas Configuration
Connection String
mongodb+srv://786ghulamdastageer_db_user:codewithmongo%402026@devtaminapi.ya8h86a.mongodb.net/
📘 Task 1 — Student Management API
📍 Server Port
PORT=5000
📂 Setup & Installation
cd Task1_StudentAPI
npm install
npm run dev
🔐 Environment Variables (.env)

Create a .env file inside Task1_StudentAPI folder.

PORT=5000
MONGODB_URI=mongodb+srv://786ghulamdastageer_db_user:codewithmongo%402026@devtaminapi.ya8h86a.mongodb.net/student_management?appName=DevtaminAPI
📌 Student API Endpoints
Method	Endpoint	Description
POST	/api/students	Create new student
GET	/api/students	Get all students
GET	/api/students/:id	Get student by ID
GET	/api/students/search?name=	Search students by name
PUT	/api/students/:id	Update complete student
PATCH	/api/students/:id	Partial update
DELETE	/api/students/:id	Delete student
PATCH	/api/students/:id/deactivate	Deactivate student
📌 Features
CRUD Operations
Student Search Functionality
Student Activation/Deactivation
MongoDB Atlas Integration
RESTful API Structure
Error Handling Middleware
📘 Task 2 — Blog Application API
📍 Server Port
PORT=5001
📂 Setup & Installation
cd Task2_BlogAPI
npm install
npm run dev
🔐 Environment Variables (.env)

Create a .env file inside Task2_BlogAPI folder.

PORT=5001
MONGODB_URI=mongodb+srv://786ghulamdastageer_db_user:codewithmongo%402026@devtaminapi.ya8h86a.mongodb.net/blog_platform?appName=DevtaminAPI
BCRYPT_ROUNDS=10
📌 User Endpoints
Method	Endpoint	Description
POST	/api/users/register	Register new user
GET	/api/users	Get all users
GET	/api/users/:id	Get user by ID
📌 Post Endpoints
Method	Endpoint	Description
POST	/api/posts	Create new post
GET	/api/posts	Get all posts
GET	/api/posts/:id	Get single post
GET	/api/posts/tag/:tag	Get posts by tag
PUT	/api/posts/:id	Update post
DELETE	/api/posts/:id	Delete post
📌 Comment Endpoints
Method	Endpoint	Description
POST	/api/posts/:postId/comments	Add comment
GET	/api/posts/:postId/comments	Get post comments
DELETE	/api/comments/:id	Delete comment
📌 Features
User Registration
Blog Post Management
Comment System
Tag-Based Filtering
Password Hashing using bcrypt
RESTful API Architecture
MongoDB Atlas Integration
▶️ Running Both Servers Together
Terminal 1
cd Task1_StudentAPI
npm run dev
Terminal 2
cd Task2_BlogAPI
npm run dev
🧪 API Testing

You can test APIs using:

Postman
Thunder Client
Insomnia
📌 Example API Base URLs
http://localhost:5000/api/students

http://localhost:5001/api/posts
