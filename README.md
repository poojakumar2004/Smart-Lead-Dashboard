# 🚀 Smart Leads Dashboard

A full-stack **Lead Management System** built using **React (Vite)** for frontend and **Node.js + Express** for backend.  
This project helps manage, track, and organize sales leads efficiently with a clean dashboard interface.

---

## 📌 Features

- 📊 Interactive dashboard for lead tracking
- ➕ Add, update, and delete leads
- 🔍 Search and filter leads
- 📈 Lead status management (New, Contacted, Converted, Rejected)
- ⚡ Fast frontend using Vite + React
- 🌐 REST API backend using Node.js & Express
- 💾 Database integration (MongoDB / JSON based depending on setup)

---

## 🏗️ Project Structure

```

Smart Lead Dashboard/
│
├── client/                # Frontend (React + Vite)
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── index.html
│   └── package.json
│
├── server/                # Backend (Node + Express)
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── server.js
│   └── package.json
│
└── README.md

````

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone (https://github.com/poojakumar2004/Smart-Lead-Dashboard)
cd smart-leads-dashboard
````

---

### 2️⃣ Setup Backend (Server)

```bash
cd server
npm install
```

Run backend:

```bash
npm start
```

Server will run on:

```
http://localhost:5000
```

---

### 3️⃣ Setup Frontend (Client)

```bash
cd client
npm install
npm run dev
```

Frontend will run on:

```
http://localhost:5173
```

---

## 🔗 API Endpoints (Example)

| Method | Endpoint       | Description     |
| ------ | -------------- | --------------- |
| GET    | /api/leads     | Get all leads   |
| POST   | /api/leads     | Create new lead |
| PUT    | /api/leads/:id | Update lead     |
| DELETE | /api/leads/:id | Delete lead     |

---

## 🛠️ Tech Stack

### Frontend:

* React.js
* Vite
* Axios
* CSS / Tailwind (if used)

### Backend:

* Node.js
* Express.js
* MongoDB (optional)
* CORS
* Dotenv

---

## 📷 Screenshots

> Add screenshots here after running the project


## 🚀 Future Improvements

* Authentication (Login/Signup)
* Role-based access (Admin/User)
* Email notifications
* Advanced analytics dashboard
* Export leads to Excel/PDF

---

## 👨‍💻 Author

**Pooja Kumar**
GitHub: [https://github.com/poojakumar]
---

## 📄 License

This project is for academic purpose and practice.
