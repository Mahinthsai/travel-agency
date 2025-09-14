Here’s a suggested improved **README.md** for your *travel-agency* project. You can adapt it (especially the image URLs) once you upload new screenshots.

---

````md
# Travel & Tourism Management System (MERN)

A full-stack application for booking travel packages, managing users, payments, and admin operations. Built with **MongoDB**, **Express**, **React**, **Node.js**.

---

## 📋 Features

- User registration / login with JWT authentication  
- Browse available travel packages  
- Book packages & make payments via Braintree  
- Admin panel to manage packages, view all bookings/payments  
- Role-based access: user vs admin  
- Environment configuration for dev & production  

---

## 📸 Screenshots

*(Drag & drop your new screenshots when editing this file. GitHub will upload them and insert the URL.)*

### Frontend

![Home Page](PUT_LINK_HERE)  
![Package Booking Page](PUT_LINK_HERE)

### Admin Panel

![Admin Dashboard](PUT_LINK_HERE)  
![Add Package Page](PUT_LINK_HERE)  
![All Payments Page](PUT_LINK_HERE)

---

## 🛠️ Setup & Installation

1. **Clone the repo**

   ```bash
   git clone https://github.com/Mahinthsai/travel-agency.git
   cd travel-agency
````

2. **Backend setup**

   ```bash
   cd backend
   npm install
   ```

   Create a `.env` file (you can rename `.env-sample`) with:

   ```
   MONGO_URL=<your MongoDB connection string>
   JWT_SECRET=<your JWT secret>
   BRAINTREE_MERCHANT_ID=<your Braintree merchant id>
   BRAINTREE_PUBLIC_KEY=<your Braintree public key>
   BRAINTREE_PRIVATE_KEY=<your Braintree private key>
   NODE_ENV_CUSTOM=development or production
   SERVER_URL=<your server url>
   ```

3. **Frontend setup**

   ```bash
   cd ../client
   npm install
   ```

   If needed, set environment variables in client (e.g. API base URL) depending on how the client is configured.

4. **Run**

   * Start backend server (from `backend`):

     ```bash
     npm run dev
     ```

   * Start frontend (from `client`):

     ```bash
     npm start
     ```

   The client usually runs on `http://localhost:3000` and server on something like `http://localhost:5000` (or as per your config).

---

## 🗂️ Project Structure

```
travel-agency/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   ├── services/
│   ├── config/
│   └── app.js / server.js
├── client/
│   ├── public/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── services/ (API calls)
│   │   └── context / state management
│   └── package.json
├── .env-sample
├── README.md
└── .gitignore
```

---

## ⚙️ CORS & Security

* Backend must enable **CORS** so that React frontend (possibly on different origin / port) can make API calls.
* Protect routes: only allow certain endpoints for admins.
* Validate user input, sanitize data, handle errors well.
* Use HTTPS in production, keep secrets safe.

---

## 🚀 Deployment (Optional Tips)

* Use environment variables in deployment environment.
* Host backend (e.g. on Heroku / AWS / DigitalOcean) and frontend (e.g. on Vercel / Netlify) or serve frontend from backend.
* Use MongoDB Atlas or other hosted DB.
* Set up proper logging / monitoring.

---

## 🤝 Contributing

If you want to contribute:

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Make changes & test
4. Push & open a Pull Request

---

## 📝 License & Credits

* This project was built by **Mahinthsai** (or your name).
* Feel free to use / modify for learning or production.
* (Optional: add license file if needed)

---

```

---

If you like, I can generate the same README with your current screenshots (from your repo) included, or suggest badges (build / license etc.) to spice it up.
::contentReference[oaicite:0]{index=0}
```
