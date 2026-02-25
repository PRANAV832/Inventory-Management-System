# 📦 Inventory Management System

![React](https://img.shields.io/badge/Frontend-React-blue)
![FastAPI](https://img.shields.io/badge/Backend-FastAPI-green)
![JWT](https://img.shields.io/badge/Auth-JWT-orange)
![License](https://img.shields.io/badge/License-Educational-lightgrey)

A Full-Stack **Inventory Management System** built to efficiently manage products, stock levels, and users with secure role-based authentication.

This project demonstrates complete frontend-backend integration using modern web technologies.

---

## 🚀 Features

### 🔐 Authentication System

* JWT-based secure login
* Role-based access control (Admin / Staff)
* Protected routes
* Token storage using LocalStorage

---

### 📊 Admin Capabilities

* Add new products
* Edit product details
* Delete products
* Manage stock levels
* Manage staff users
* Full dashboard access

---

### 🧑‍💼 Staff Capabilities

* View product inventory
* Update stock quantity
* Restricted dashboard access

---

## 🛠️ Tech Stack

### 💻 Frontend

* React (Vite)
* JavaScript (ES6+)
* Fetch API
* LocalStorage
* Responsive UI

### ⚙️ Backend

* FastAPI (Python)
* JWT Authentication
* RESTful APIs
* SQLite / PostgreSQL
* Uvicorn Server

---

## 📁 Project Structure

```
InventoryManagementSystem/
│
├── Frontend/        # React + Vite frontend
├── backend/         # FastAPI backend
└── README.md
```

---

## ⚙️ Installation & Setup Guide

### 1️⃣ Clone Repository

```bash
git clone https://github.com/PRANAV832/Inventory-Management-System.git
cd Inventory-Management-System
```

---

## 🔹 Backend Setup

```bash
cd backend
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

Backend runs on:

```
http://localhost:8000
```

---

## 🔹 Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

Frontend runs on:

```
http://localhost:5173
```

---

## 🔑 Environment Variables

Create a `.env` file inside the **Frontend** folder:

```
VITE_BACKEND_URL=http://localhost:8000
```

---

## 🔄 Application Flow

1. User logs in with credentials.
2. Backend verifies credentials.
3. JWT token is generated.
4. Token is stored in LocalStorage.
5. User is redirected based on role.
6. Protected routes validate token before access.

---

## 📌 API Overview

| Method | Endpoint       | Description         |
| ------ | -------------- | ------------------- |
| POST   | /login         | Authenticate user   |
| GET    | /products      | Get all products    |
| POST   | /products      | Add product (Admin) |
| PUT    | /products/{id} | Update product      |
| DELETE | /products/{id} | Delete product      |

---

## 🧠 Learning Outcomes

* Full-stack architecture
* JWT authentication implementation
* Role-based authorization
* REST API design
* Frontend-backend integration
* Environment variable handling
* Git & GitHub version control


## 👨‍💻 Author

**Pranav Nair**

---

## 📜 License

This project is developed for educational purposes.

---
