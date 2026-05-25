# 📝 Blog Platform with Comments

A full-stack blogging platform where users can register, login, create blog posts, and interact through comments.

---

## 🚀 Features

- 🔐 User Authentication (Register / Login with JWT)
- 📝 Create, Edit, Delete Blog Posts
- 💬 Comment system for each post
- 👤 User-specific post management
- 🔒 Protected routes using authentication
- 📱 Responsive UI (frontend-ready)
- ⚡ RESTful API backend

---

## 🛠️ Tech Stack

### Frontend
- React.js (or HTML/CSS/JS if basic version)
- Axios (API calls)
- React Router

### Backend
- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT (Authentication)
- Bcrypt.js (Password hashing)

---

## 📁 Project Structure
Blog-Platform/
│
├── backend/
│ ├── models/
│ ├── routes/
│ ├── middleware/
│ ├── server.js
│ └── .env
│
├── frontend/
│ ├── src/
│ ├── public/
│ └── package.json
│
└── README.md


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/blog-platform.git
cd blog-platform
2️⃣ Backend setup
cd backend
npm install

Create .env file:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

Run backend:

npm start
3️⃣ Frontend setup
cd frontend
npm install
npm run dev
🔐 Authentication Flow
User registers with username, email, password
Password is hashed using bcrypt
Login returns a JWT token
Token is stored in localStorage
Protected routes use token verification
💬 API Endpoints
Auth Routes
POST /api/auth/register → Register user
POST /api/auth/login → Login user
Blog Routes
GET /api/posts → Get all posts
POST /api/posts → Create post
PUT /api/posts/:id → Update post
DELETE /api/posts/:id → Delete post
Comment Routes
POST /api/comments/:postId → Add comment
GET /api/comments/:postId → Get comments
📌 Future Improvements
Like/Dislike system 👍👎
Image upload for posts
User profiles
Pagination & search
Rich text editor
👨‍💻 Author

Built with ❤️ by Sabiya Kousar

📜 License

This project is open-source and free to use.
