# 🚦 RouteX — AI-Powered Traffic Intelligence Platform

<img width="193" height="45" alt="image" src="https://github.com/user-attachments/assets/14a2158c-7292-4932-95de-d5e869b9fe58" />

![React](https://img.shields.io/badge/Frontend-React-blue)
![Spring Boot](https://img.shields.io/badge/Backend-SpringBoot-green)
![FastAPI](https://img.shields.io/badge/ML-FastAPI-teal)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-blue)
![Redis](https://img.shields.io/badge/Cache-Redis-red)
![AWS](https://img.shields.io/badge/Deployment-AWS-orange)
![WebSocket](https://img.shields.io/badge/Realtime-WebSocket-purple)

RouteX is a full-stack AI-powered Traffic Intelligence Platform that predicts traffic congestion, provides intelligent route recommendations, delivers real-time alerts, and offers an AI traffic assistant to help users make better travel decisions.

The platform combines Machine Learning, Real-Time WebSockets, Redis Caching, and Cloud Deployment to create a production-ready traffic management solution.

---

## 🚀 Live Demo

* 🌐 Frontend: (http://43.205.209.209)
* 🔗 Backend API: (http://43.205.209.209)
* 📹 Demo Video: (https://drive.google.com/file/d/1trsAikNASzP8kqXnpEE10rLG2sgtY696/view?usp=drivesdk)

---

# 📌 Table of Contents

* Overview
* Features
* System Architecture
* Tech Stack
* Getting Started
* Environment Variables
* API Reference
* AI Pipeline
* Project Structure
* Deployment
* Future Enhancements

---

# 🌍 Overview

Urban traffic congestion impacts millions of commuters every day. RouteX leverages Machine Learning and Real-Time Data Processing to provide:

* Traffic prediction and route intelligence
* AI-powered traffic assistance
* Historical traffic analytics
* Real-time alert notifications
* Ecosystem and congestion monitoring

The system enables users to proactively plan travel routes and understand future traffic conditions before they start their journey.

---

# ✨ Features

## 🤖 AI Traffic Assistant

* Intelligent traffic-related conversations
* Route recommendations
* Traffic insights and explanations
* AI-generated travel suggestions

---

## 🚦 Traffic Prediction Engine

* Predict congestion levels
* Estimate travel duration
* Traffic confidence scoring
* Route optimization

---

## 📊 Analytics Dashboard

* Historical traffic trends
* Weekly traffic reports
* Route performance analysis
* User prediction history

---

## 🔔 Real-Time Notifications

* WebSocket-based live alerts
* Congestion warnings
* Traffic incidents
* Route advisories

---

## 🔐 Authentication & Security

* JWT Authentication
* Role-based authorization
* Secure password encryption
* Session management

---

## ⚡ Performance Optimization

* Redis caching layer
* Optimized API responses
* Efficient database querying
* Reduced backend latency

---

# 🏗 System Architecture

```text
┌─────────────────────────────────────────┐
│             React Frontend              │
└────────────────────┬────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────┐
│               Nginx Proxy               │
└────────────────────┬────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────┐
│          Spring Boot Backend            │
│                                         │
│  Authentication                         │
│  Traffic Prediction Service             │
│  Analytics Service                      │
│  Alert Management                       │
│  WebSocket Notifications                │
└───────┬─────────────────┬───────────────┘
        │                 │
        ▼                 ▼

┌──────────────┐   ┌───────────────┐
│ PostgreSQL  │   │ Redis Cache   │
└──────────────┘   └───────────────┘
        │                
        ▼
┌─────────────────────────────────────────┐
│           FastAPI ML Service            │
│                                         │
│ Traffic Prediction Models               │
│ Route Intelligence Engine               │
└─────────────────────────────────────────┘
```

# 🛠 Tech Stack

## Frontend

| Technology     | Purpose                 |
| -------------- | ----------------------- |
| React.js       | User Interface          |
| Vite           | Build Tool              |
| Tailwind CSS   | Styling                 |
| Axios          | API Communication       |
| SockJS + STOMP | WebSocket Communication |

---

## Backend

| Technology         | Purpose |
| ------------------ | ------- |
| Java 21            |         |
| Spring Boot        |         |
| Spring Security    |         |
| JWT Authentication |         |
| Spring Data JPA    |         |
| Hibernate          |         |
| Maven              |         |

---

## Machine Learning

| Technology   | Purpose |
| ------------ | ------- |
| FastAPI      |         |
| Python       |         |
| Scikit-Learn |         |
| Pandas       |         |
| NumPy        |         |

---

## Database & Cache

| Technology            | Purpose |
| --------------------- | ------- |
| PostgreSQL (Supabase) |         |
| Redis                 |         |

---

## Cloud & DevOps

| Technology | Purpose |
| ---------- | ------- |
| AWS EC2    |         |
| Nginx      |         |
| GitHub     |         |
| Linux      |         |

---

# 🚀 Getting Started

## Prerequisites

* Java 21+
* Python 3.11+
* Node.js 18+
* PostgreSQL
* Redis

---

## Clone Repository

```bash
git clone https://github.com/yourusername/RouteX.git
cd RouteX
```

## Backend Setup

```bash
cd backend

mvn clean install
mvn spring-boot:run
```

Backend runs on:

```text
http://localhost:8080
```

---

## Frontend Setup

```bash
cd frontend

npm install
npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

---

## ML Service Setup

```bash
cd ml-service

pip install -r requirements.txt

uvicorn main:app --reload
```

ML Service runs on:

```text
http://localhost:8000
```

---

# 🔧 Environment Variables

## Backend

```env
DB_URL=
DB_USERNAME=
DB_PASSWORD=

REDIS_HOST=
REDIS_PORT=
REDIS_PASSWORD=

JWT_SECRET=

FASTAPI_URL=http://localhost:8000
```

## Frontend

```env
VITE_API_URL=http://localhost:8080
```

---

# 📸 Screenshots

## Dashboard

<img width="1917" height="962" alt="image" src="https://github.com/user-attachments/assets/fc416d00-0c3c-4209-bfff-4f91a6b12d14" />


## AI Assistant

<img width="1882" height="926" alt="image" src="https://github.com/user-attachments/assets/596c952e-2979-4196-a6e4-da35b84f5155" />


## Traffic Prediction

<img width="1730" height="972" alt="image" src="https://github.com/user-attachments/assets/0152133e-2b52-47fe-bc11-875b292cb200" />


## Alerts System

<img width="497" height="601" alt="image" src="https://github.com/user-attachments/assets/3958128c-7db1-46a6-95d6-c8e062d39ccd" />


---

# ☁️ Deployment

### Frontend

* React Build
* Hosted on AWS EC2
* Served through Nginx

### Backend

* Spring Boot JAR
* Systemd Service
* Reverse Proxy via Nginx

### ML Service

* FastAPI
* Uvicorn
* Systemd Service

---

# 🔮 Future Enhancements

* Google Maps Integration
* Live Traffic APIs
* Route Visualization
* Mobile Application
* AI Voice Assistant
* Advanced Predictive Analytics

---

# 👨‍💻 Author

Love Yadav

Full Stack Developer | Java Developer | AI Enthusiast

* LinkedIn: (https://www.linkedin.com/in/love-yadav-39b758343/)
* GitHub: (https://github.com/loveyadav8478-blip)

---

⭐ If you found this project interesting, consider giving it a star.
