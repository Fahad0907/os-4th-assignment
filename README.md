# 4th assignment

This project contains a **Django backend (Dockerized)** and a **React frontend (Vite build)** deployed on Ubuntu servers using **Nginx**.

---

## 📁 Screenshots

All screenshots are stored in the `/ss` folder:

- `/ss/database.png` → Database setup confirmation  
- `/ss/backend-end-nginx.png` → Backend Nginx configuration  
- `/ss/backend-running.png` → Backend running status  
- `/ss/front-end.png` → Frontend running status  

---

## ⚙️ Backend (Django + Docker + Nginx)

- Django runs inside a Docker container
- Gunicorn used as application server
- Nginx acts as reverse proxy

### 🔧 Flow
Client → Nginx → Docker (Gunicorn) → Django API

### 📸 Evidence
See:
- `ss/backend-end-nginx.png`
- `ss/backend-running.png`
- `ss/database.png`

---

## 🎨 Frontend (React Vite + Nginx)

- Built using Vite (`dist/`)
- Served as static files via Nginx

### 🔧 Flow
Client → Nginx → React static build

### 📸 Evidence
See:
- `ss/front-end.png`

---

## 🌐 Nginx Role

- Backend server: Reverse proxy to Django (port 8000)
- Frontend server: Serves React static files
- Handles routing for production deployment

---

## 🚀 Summary

- Backend: Django + Docker + Gunicorn + Nginx  
- Frontend: React (Vite build) + Nginx  
- Communication: REST API between frontend and backend  

---

## 📌 Notes

- Ensure ports **80/443** are open in security group
- HTTPS can be enabled using **Certbot**
- Static files are served via Nginx in production
