# 🔋 Vehicle Battery Tracker

A secure full-stack Vehicle Battery Tracking System built using the MERN stack.

This application allows users to securely register, log in, and manage vehicle battery-related records. Each vehicle entry is linked to its owner, ensuring strict data isolation and protected access.

This project was developed as a capstone implementation focusing on authentication, protected routes, ownership-based data modeling, and full-stack integration.

---
## 🎥 Lecture Recordings

**Morning Session Recording:**  
🔗 https://www.youtube.com/watch?v=dnn6cKhymy8

**Afternoon Session Recording:**  
🔗 https://www.youtube.com/watch?v=fi3TBTZCVyM

---

**Morning Session Recording:**  
🔗 https://www.youtube.com/watch?v=wo67jkxt1jc

**Afternoon Session Recording:**  
🔗 https://www.youtube.com/watch?v=XHrDGC6p-Zg

---

## 🚀 Features

### 🔐 Authentication
- User Registration
- User Login
- JWT-based authentication
- Password hashing using bcrypt
- Persistent login via localStorage
- Protected frontend & backend routes

### 🚗 Vehicle Management
- Add vehicle records
- Fetch user-specific vehicle data
- Ownership enforcement (each vehicle belongs to a user)
- Secure dashboard displaying only authorized data

### 🛡 Security Architecture
- JWT verification middleware
- Token-based request authorization
- Backend ownership validation
- Data isolation per authenticated user
- 401 handling for unauthorized access

---

## 🏗 System Architecture

### Backend (Node.js + Express + MongoDB)

-   backend/
-   config/
-   db.js
-   models/
-   User.js
-   Vehicle.js
-   routes/
-   auth.js
-   vehicle.js
-   middleware/
-   auth.js
-   server.js

### Frontend (React + Vite)

-   frontend/
-   src/
-   pages/
-   Login.jsx
-   Register.jsx
-   Dashboard.jsx
-   components/
-   Navbar.jsx
-   VehicleCard.jsx
-   VehicleForm.jsx
-   context/
-   AuthContext.jsx
-   services/
-   api.js
-   App.jsx


---

## 🔄 Application Flow

1. User registers → password is hashed and stored securely.
2. User logs in → JWT token is generated.
3. Token is stored in localStorage.
4. Axios interceptor automatically attaches token to requests.
5. Backend middleware verifies token.
6. Vehicle records are created with user ownership.
7. Dashboard fetches and displays user-specific battery data.
8. Data persists in MongoDB.

---

## 🔑 Core Technical Concepts Implemented

- One-to-Many relationship (User → Vehicles)
- Ownership-based access control
- Stateless authentication using JWT
- Route protection on frontend and backend
- React Context API for global authentication state
- Axios interceptors for automatic token injection
- Persistent database storage

---

## 🧪 How to Run Locally

### 1️⃣ Clone Repository

```bash
git clone <your-repo-url>
cd vehicle-battery-tracker 
```

### 2️⃣ Setup Backend

```bash
cd backend
npm install
```

- Create a .env file:

```bash
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

- Run backend:

```bash
npm run dev
```

### 3️⃣ Setup Frontend

```bash
cd frontend
npm install
npm run dev
```

- Frontend runs on:

```bash
http://localhost:5173
```

- Backend runs on:

```bash
http://localhost:5000
```

### ✅ MVP Status

- Authentication implemented
- Protected routes working
- Ownership enforcement verified
- Dashboard loads user-specific data
- Data persistence confirmed
- Full flow tested and stabilized
- This project represents a production-style full-stack foundation.

### 📈 Future Enhancements

- Edit & delete vehicle entries
- Battery health tracking metrics
- Battery replacement history
- Alerts & notifications
- Admin dashboard
- Role-based access control
- Deployment to cloud (Render / Vercel)

### 🎯 What This Project Demonstrates

- Clean separation of concerns
- Secure API design
- Full-stack authentication flow
- Data ownership modeling
- Scalable folder structure
- Real-world application architecture
