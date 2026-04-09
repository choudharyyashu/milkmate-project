# 🥛 MilkMate – Dairy Management and Milk Delivery

MilkMate is a web-based milk delivery management platform built for dairies, milkmen, and customers to streamline the process of milk distribution. It supports role-based login and operations like order tracking, customer management, product listings, and cart handling.

**Live Site:** [https://milkmate.onrender.com](https://milkmate.onrender.com)

---

## 🚀 Features

- 🔐 **Role-based Authentication** (Customer, Dairy, Milkman)
- 🧾 **Product Listings** and Cart System
- 📦 **Order Management** for Customers
- 📊 **Dashboard** for Dairy and Milkman
- 🔁 **Flash Messages** and User Feedback
- 🧠 Session handling with `express-session` and MongoDB store
- 📱 Fully responsive UI using EJS + custom CSS

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, EJS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Atlas)
- **Other Libraries:**
  - `express-session`, `connect-mongo`, `mongoose`, `method-override`
  - `connect-flash` for user alerts
  - `dotenv` for environment variables

---

## 📋 Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd MilkMate-main
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Environment Variables:**
   Create a `.env` file in the root directory:
   ```env
   PORT=3000
   MONGO_URI=mongodb://localhost:27017/milkmate
   SESSION_SECRET=your_secret_key_here
   ```

   - Replace `MONGO_URI` with your MongoDB connection string.
   - Choose a strong `SESSION_SECRET` for security.

4. **Run the application:**
   ```bash
   npm start
   ```

   The app will start on `http://localhost:3000` (or the port specified in `.env`).

---

## 🔧 Troubleshooting

- **Port already in use:** If port 3000 is busy, change `PORT` in `.env` to another value like 3001.
- **MongoDB connection error:** Ensure MongoDB is running locally or update `MONGO_URI` for Atlas.
- **Login issues:** Passwords are stored in plain text; consider implementing hashing for production.
- **Signup errors:** The signup uses `.insertOne()` which may not trigger Mongoose validation; use `.save()` for better error handling.

---

## 🧠 Learning Goals

- Backend routing and MVC pattern
- Role-based access control
- CRUD operations in MongoDB
- Middleware and session management
- Responsive EJS templating

---

## 🙋‍♂️ Author

- Yashwant Choudhary
- **Email**: yashuchoudhary3621@gmail.com
