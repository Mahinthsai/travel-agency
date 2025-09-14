# 🌍 Travel & Tourism Management System (MERN)

A modern full-stack web application for booking travel packages, managing users, payments, and admin operations.  
Built with **MongoDB**, **Express.js**, **React.js**, and **Node.js**.

---

## ✨ Features

✅ User registration & login with JWT authentication  
✅ Browse and search travel packages  
✅ Book packages & make secure payments via **Braintree**  
✅ Admin panel to manage packages, bookings, and payments  
✅ Role-based access: **User** vs **Admin**  
✅ Environment configuration for dev & production

---

## 📸 Screenshots

### User Interface
![Home Page](https://github.com/user-attachments/assets/c4250b00-19f0-4826-9088-b627b59c1402)  
![Package Booking Page](https://github.com/user-attachments/assets/03c245ca-a30c-41bd-8ece-4a6e2c3160e8)

### Admin Panel
![Admin Dashboard](https://github.com/user-attachments/assets/46994168-d698-4a71-9dcc-157a06fce795)  
![Add Package Page](https://github.com/user-attachments/assets/e4ee24da-2093-4083-b81d-0d0502ac28f5)

---

## 🏗️ Project Architecture

~~~text
Frontend (React)
    |
    |-- REST API Calls
    v
Backend (Node.js + Express)
    |
    |-- Authentication & Authorization (JWT, Roles)
    |-- Package / Booking / Payment Controllers
    v
Database (MongoDB)
    |
    |-- Collections: Users, Packages, Bookings, Payments

External Services:
    - Braintree (Payments)
    - Email / Notifications (Optional)
~~~

---

## ⚙️ Setup & Installation

1. **Clone the repository**

~~~bash
git clone https://github.com/Mahinthsai/travel-agency.git
cd travel-agency
~~~

2. **Backend setup**

~~~bash
cd backend
npm install
~~~

Create a `.env` file (you can copy `.env-sample`) and add:

~~~env
MONGO_URL=your_mongo_url
JWT_SECRET=your_secret
BRAINTREE_MERCHANT_ID=your_braintree_id
BRAINTREE_PUBLIC_KEY=your_braintree_public_key
BRAINTREE_PRIVATE_KEY=your_braintree_private_key
NODE_ENV_CUSTOM=development
SERVER_URL=http://localhost:5000
~~~

3. **Frontend setup**

~~~bash
cd ../client
npm install
npm start
~~~

4. **Run the project**

- Backend: `npm run dev` (from `backend` folder)  
- Frontend: `npm start` (from `client` folder)

By default:  
- Frontend → http://localhost:3000  
- Backend → http://localhost:5000

---

## 🗂️ Project Structure

~~~text
travel-agency/
├── backend/
│   ├── controllers/     # Business logic
│   ├── models/          # Mongoose schemas
│   ├── routes/          # API routes
│   ├── middlewares/     # Auth, validation
│   ├── services/        # Payment, email helpers
│   ├── config/          # DB & app config
│   └── server.js        # App entry point
│
├── client/
│   ├── public/
│   ├── src/
│   │   ├── components/  # Reusable UI parts
│   │   ├── pages/       # Screens
│   │   ├── services/    # API calls
│   │   └── context/     # State management
│   └── package.json
│
└── README.md
~~~

---

## 🔒 Security & Best Practices

- Enable **CORS** on backend to allow React frontend requests  
- Store secrets in `.env` (never commit them)  
- Use password hashing (bcrypt) for users  
- Validate and sanitize user input to prevent NoSQL injection  
- Use HTTPS in production

---

## 🚀 Deployment Tips

- Use **MongoDB Atlas** for a hosted database  
- Host backend on **Render / Railway / AWS / Heroku**  
- Host frontend on **Netlify / Vercel** (or serve static build from backend)  
- Configure environment variables in your hosting platform  
- Set up basic CI/CD for automated deployments

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo  
2. Create a feature branch (`git checkout -b feature/new-feature`)  
3. Commit changes (`git commit -m "Add new feature"`)  
4. Push (`git push origin feature/new-feature`)  
5. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to use and modify for learning or production.

---

👨‍💻 Developed by **Mahinth Sai**
