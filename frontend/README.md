🛒 OneCart – MERN E-Commerce Platform

**OneCart** is a complete fashion-centric e-commerce web application built using the **MERN stack**. It features a responsive frontend for customers, a secure admin dashboard, and a scalable backend API — all designed to simulate real-world e-commerce systems during a hands-on virtual internship.

---

## 🧩 Key Features

- 🛍️ **Fashion-Focused UI** – Bold homepage with curated collections
- 🛒 **Cart Management** – Add to cart, remove, total calculation
- 🧑‍💼 **Admin Panel** – Add/delete products via a protected dashboard
- 🔐 **Secure Routing** – Backend API secured with route-level protection
- 📦 **Product Categories** – Categorized product listing for easy browsing
- 🔄 **Order Flow (WIP)** – Cart to checkout with order placeholders
- ⚡ **Fast UX** – Vite-powered frontend and admin dashboard
- 🌐 **Seamless Architecture** – Frontend, admin, and backend are modular

---

## 🏗️ Technical Architecture

### Frontend (React + Vite)

- Built using React with Vite bundler for blazing-fast performance
- Uses **Context API** for state (cart, auth)
- Components: `Nav`, `Card`, `Hero`, `Footer`, `CategoryBanner`, etc.
- Firebase setup ready for user auth
- Responsive mobile-first design

### Admin (React + Vite)

- Separate admin dashboard app
- Add new products with image, price, category, and description
- Delete products with one click
- Clean and modern dashboard UI

### Backend (Node.js + Express)

- RESTful API built with Express.js
- Mongoose + MongoDB for database
- Product and user model setup
- Protected routes for admin
- Environment-based config system

---

## 🧠 Design Decisions

### Modular Foldering

Each app (frontend, backend, admin) is separate — scalable for large production systems.

### Vite over CRA

Vite ensures fast hot module replacement and dev build time.

### Context API vs Redux

Lightweight Context API was used instead of Redux for simplicity and speed.

### Secure Backend Routing

Admin routes are separated and protected for future JWT-based auth.

---

## 🗃️ Project Structure

tutedude/
├── client/                 # React frontend
│   ├── public/             # Static files
│   ├── src/                # Source code
│   │   ├── components/     # React components
│   │   │   ├── layout/     # Layout components (Header, Footer)
│   │   │   ├── routing/    # Routing components
│   │   │   └── video/      # Video-related components
│   │   ├── contexts/       # React contexts
│   │   ├── hooks/          # Custom hooks
│   │   ├── pages/          # Page components
│   │   ├── services/       # API services
│   │   ├── styles/         # Global styles
│   │   ├── utils/          # Utility functions
│   │   └── App.js          # Main App component
│   └── package.json        # Frontend dependencies
├── server/                 # Node.js backend
│   ├── config/             # Configuration files
│   ├── controllers/        # Request handlers
│   ├── db/                 # Database setup and migrations
│   ├── middleware/         # Express middleware
│   ├── models/             # Data models
│   ├── routes/             # API routes
│   ├── services/           # Business logic
│   ├── utils/              # Utility functions
│   └── server.js           # Main server file
└── README.md               # Project documentation



## ⚙️ Setup Instructions

### Prerequisites

- Node.js (v14+)
- MongoDB
- npm or yarn

---

### 🖥️ Backend Setup

```bash
cd backend
npm install
Create a .env file with:

env
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
Then start the server:

bash
Copy
Edit
npm start
API runs on: http://localhost:5000

💻 Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm run dev
Runs at: http://localhost:5173

🧑‍💼 Admin Panel Setup
bash
Copy
Edit
cd admin
npm install
npm run dev
Runs at: http://localhost:5174

📡 API Endpoints
Products
GET /api/products – Get all products

POST /api/products – Add a new product (admin)

DELETE /api/products/:id – Delete product (admin)

Users (Coming Soon)
POST /api/auth/register

POST /api/auth/login

🛠️ Technologies Used
Frontend & Admin
React.js

Vite

React Router

Context API

Firebase (Auth Ready)

Tailwind / CSS

Backend
Node.js

Express.js

MongoDB

Mongoose

dotenv

🚀 Future Enhancements
🔐 JWT-based user authentication

💳 Razorpay or Stripe integration

⭐ Product rating & review system

📦 Order history & user profile

📈 Admin analytics dashboard

📱 Mobile responsive PWA

👨‍💻 Contributors
Archit Kumar – Full Stack Developer
