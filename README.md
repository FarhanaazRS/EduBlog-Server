# EduBlog Server 📚🖥️

EduBlog Server is a powerful backend system for a blogging and study platform. It handles blog posts, user management, comments, and study materials efficiently using Node.js and Express.

---

## 🚀 Features

- ✍️ Blog post creation, retrieval, updating, and deletion
- 🧑‍💻 User registration and authentication
- 💬 Comment system for interactive blogs
- 📘 Study material upload and retrieval support
- 📦 RESTful API endpoints
- 🌐 Vercel support for serverless deployment

---

## 🧱 Tech Stack

- **Node.js** & **Express.js** – backend server
- **MongoDB** – NoSQL database
- **Mongoose** – ODM for MongoDB
- **Vercel** – Deployment
- **JSON Web Tokens (JWT)** – Authentication
- **dotenv** – Environment variable management

---

## 📁 Project Structure

```
edublog-server/
│
├── edublog-server-main/
│   ├── .gitattributes
│   ├── .gitignore
│   ├── index.js                  # Entry point
│   ├── package-lock.json
│   ├── package.json              # Project dependencies
│   ├── vercel.json               # Vercel deployment config
│   └── routes/
│       ├── blogRoutes.js
│       ├── commentRoutes.js
│       ├── studyMaterials.js
│       └── userRoutes.js
```

---

## 🛠️ Getting Started

### 📦 Prerequisites

- Node.js and npm installed
- MongoDB database (local or Atlas)
- Vercel account (optional for deployment)

### 🔧 Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/edublog-server.git
cd edublog-server/edublog-server-main
```

2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file in the root:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

4. Start the server:

```bash
npm start
```

Server will run at `http://localhost:5000`.

---

## 📚 API Endpoints

### 🔑 Auth
- `POST /api/users/register` - Register new user
- `POST /api/users/login` - Login and get token

### 📘 Blog
- `POST /api/blogs` - Create new blog
- `GET /api/blogs` - Get all blogs
- `GET /api/blogs/:id` - Get blog by ID
- `PUT /api/blogs/:id` - Update blog
- `DELETE /api/blogs/:id` - Delete blog

### 💬 Comments
- `POST /api/comments` - Add comment
- `GET /api/comments/:blogId` - Get comments for blog

### 📂 Study Materials
- `POST /api/materials` - Upload study material
- `GET /api/materials` - Get all study materials

---

## ⚙️ Deployment

This project supports deployment on [Vercel](https://vercel.com):

1. Configure the `vercel.json` file.
2. Deploy via CLI or GitHub integration.

---

