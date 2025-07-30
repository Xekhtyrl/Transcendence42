# Transcendence42 🏓

**Final 42 common‑core project: a real‑time multiplayer Pong SPA with chat and matchmaking.**

---

## 🎯 Overview

* Full-stack single-page application (SPA) allowing users to play **Pong** online in real time
* Built with **multiple services**: chat, user management, matchmaking, game engine
* Includes **friend system**, **AI Player**, **private messaging**, and **remote multiplayer**

---

## 🚀 Features

* **Multiplayer Pong gameplay** in competitive and friendly modes
* **Real-time chat and possibility to start a game** with channels and private messages
* **Matchmaking system** including non-tournament and tournament modes
* **User profiles** with avatars, stats, and game history
* **AI Pong** 1v1 local pong game against a AI
* **Server Side Pong** Game update given by the front_end and calculate by the back-end implementation.
* **GDPR-compliant authentication**, including optional Two-Factor Authentication (2FA) ([GitHub][5])

---

## 🧱 Tech Stack

| Layer      | Technology                                                   |
| ---------- | ------------------------------------------------------------ |
| Backend    | Django (Python)                                              |
| Frontend   | Vanilla JavaScript and Bootstrap                             |
| Database   | PostgreSQL                                                   |
| API        | Web-Socket                                                   |
| Deployment | Docker, NGINX, Docker Compose                                |
| Real-Time  | WebSocket (Channels)                                         |

---

## ⚙️ Installation & Setup

!!! As there is no .env file the program won't run

```bash
git clone https://github.com/Xekhtyrl/Transcendence42.git
cd Transcendence42
make
```

Once services are running, open your browser at:

* `https://localhost:8443` (frontend served via NGINX)

---

## 🛠 Usage

* Create an account to log in, or log in
* Select Game Option (Local, Multi (x4) or Tournament)
* View profiles, Chats, and manage chats/friends

---

## 🔍 Architecture & Structure

* Organized into Three Container: Nginx, PostgreSQL and Django
* Services typically include: user-management, matchmaking, game-server, stats, AI, Chats, frontend
* Configured via **docker-compose.yml** and environment variables
* Communication between back and front end through HTTP APIs and WebSocket channels

---

## 🧪 Testing & Deployment

* Use `make` for local setup
* Create `dev.env` in a `.env` folder and insert:

  ```text
  SECRET_KEY =
  DEBUG =
  ALLOWED_HOSTS =
  POSTGRES_USER =
  DB =
  DB_PASSWORD =
  POSTGRES_CONTAINER_NAME =
  POSTGRES_PORT =
  CHNL_DB =
  CHNL_DB_USER =
  CHNL_DB_PASSWORD =
  CHNL_POSTGRES_CONTAINER_NAME =
  CHNL_POSTGRES_PORT =
  DJANGO_SUPERUSER_USERNAME =
  DJANGO_SUPERUSER_EMAIL =
  DJANGO_SUPERUSER_PASSWORD =
  POSTGRES_HOST_AUTH_METHOD =
  POSTGRES_LISTEN_ADDRESSES =
  POSTGRES_PORT =
  ```
* For production deployment, configure NGINX with TLS, scale services via Docker orchestration

---

## 📚 References & Influences

This project follows the 42 guideline for Transcendance.

---

## ✨ Why This Project Matters

* Demonstrates **full-stack development skills** including frontend, backend, real-time communication, deployment, and security
* Covers **microservice architecture**, Docker orchestration, asynchronous event handling
* Mirrors production-grade SPA patterns, real-time game programming, and social user experiences

---
