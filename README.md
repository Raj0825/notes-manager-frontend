# 📘 Notes Manager – Frontend

A simple frontend for the **Notes Manager** application, built using **HTML, CSS, and JavaScript**, and deployed using **GitHub Pages**.

This frontend communicates with a publicly deployed **Spring Boot REST API**.

---

## 🔗 Live Demo

👉 **Frontend (UI):**

```
https://rajo825.github.io/notes-manager-frontend/
```

👉 **Backend (API):**

```
https://notes-manager-backend-7yp6.onrender.com
```

> ⚠️ Note: The backend runs on a free hosting tier and may take **30–60 seconds** to respond on the first request due to cold start.

---

## 🛠 Tech Stack

### Frontend

* HTML
* CSS
* JavaScript (Vanilla JS)
* Fetch API

### Backend (separate repository)

* Java
* Spring Boot
* Spring Data JPA
* H2 Database
* Docker
* Render (deployment)

---

## ✨ Features

* Create notes
* View all notes
* Delete notes
* Responsive web UI
* Communicates with REST APIs using JSON

---

## 📂 Project Structure

```
notes-manager-frontend/
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## ⚙️ How It Works

* The frontend is a **static web application** hosted on GitHub Pages
* All data operations are handled by a **Spring Boot backend**
* API requests are sent using the Fetch API
* The frontend does **not** store any data locally

---

## ⚠️ Important Limitations (Intentional)

This project is designed as a **demo application**, not a production system.

* No user authentication
* All notes are publicly accessible
* Anyone can add or delete notes
* Data may reset when the backend restarts (H2 + free hosting)

These trade-offs were made to keep the scope focused on:

* REST API integration
* Deployment
* End-to-end system understanding

---

## 🧠 Learning Outcomes

* Consuming REST APIs from a frontend
* Handling asynchronous requests using Fetch
* Deploying static sites with GitHub Pages
* Integrating frontend with a cloud-deployed backend
* Understanding real-world deployment issues (cold starts, CORS, environment separation)

---

## 🚀 Future Improvements

* User authentication and authorization
* Per-user note ownership
* Persistent database (PostgreSQL/MySQL)
* Improved mobile responsiveness
* Pagination and search

---

## 👤 Author

**Raj Shah**
Engineering Student | Java & Spring Boot Learner

---
