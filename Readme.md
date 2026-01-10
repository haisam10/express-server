# 🚀 Express Server

A simple **Node.js + Express.js** backend server for learning and practicing basic routing and API development.

---

## 📌 Project Overview

This project demonstrates how to create a basic backend server using **Express.js**. It handles HTTP requests, serves simple pages, and provides sample API endpoints (such as student data).

This repository is suitable for:

* Beginners learning Express.js
* Understanding routing and REST-style APIs
* Practicing backend fundamentals

---

## 🛠️ Technologies Used

* **Node.js**
* **Express.js**
* JavaScript (CommonJS)

---

## 📂 Project Structure

```
express-server/
├── models/            # Data models (students data)
├── db.js              # Data / database logic
├── index.js           # Express routes & API logic
├── package.json       # Project dependencies & scripts
├── package-lock.json  # Dependency lock file
└── README.md          # Documentation
```

---

## ⚙️ Installation & Setup

### ✅ Prerequisites

* Node.js (v14 or higher recommended)
* npm (comes with Node.js)

---

### 🔧 Setup Steps

1️⃣ **Clone the repository**

```bash
git clone https://github.com/haisam10/express-server.git
cd express-server
```

2️⃣ **Install dependencies**

```bash
npm install
```

3️⃣ **Run the server**

```bash
node server.js
```

4️⃣ **Server will start on:**

```
http://localhost:5000
```

(Default port: **5000**)

---

## 🌐 API Routes & Endpoints

### 🏠 Root Route

**GET /**
Returns a basic welcome response.

```
http://localhost:5000/
```

---

### 📱 Phone Page

**GET /phone**
Returns a simple HTML/text response.

```
http://localhost:5000/phone
```

---

## 👨‍🎓 Student APIs

### 📄 Get All Students

**GET /students**
Returns a list of all students.

```
http://localhost:5000/students
```

---

### 🔍 Get Student by ID

**GET /students/:id**
Returns student information by ID.

```
http://localhost:5000/students/1
```

---

### 🔎 Get Student by Name

**GET /students/name/:name**
Returns student information by name.

```
http://localhost:5000/students/name/haisam
```

---

## 📄 Static Pages

### ℹ️ About Page

**GET /about**

```
http://localhost:5000/about
```

### ☎️ Contact Page

**GET /contact**

```
http://localhost:5000/contact
```

---

## 🧪 Testing

You can test the APIs using:

* Browser
* Postman
* Insomnia
* cURL

Example:

```bash
curl http://localhost:5000/students
```

---

## 💡 Notes

* This project uses **static data** (no real database)
* Designed for learning and practice
* Easily extendable with MongoDB or MySQL

---

## 🚀 Future Improvements

* Add POST, PUT, DELETE APIs
* Integrate MongoDB / MySQL
* Add authentication (JWT)
* Environment variables (.env)

---

## 👤 Author

**Md Haisam Hoque**
GitHub: [https://github.com/haisam10](https://github.com/haisam10)

---

⭐ If you find this project helpful, don’t forget to give it a star!

