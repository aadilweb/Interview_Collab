# 🚀 InterviewCollab

### Real-Time Collaborative Technical Interview Platform

[![React](https://img.shields.io/badge/React-2023?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)

---

## 📌 About

**InterviewCollab** is a real-time collaborative platform designed to simulate technical interview environments.

The platform brings together collaborative coding, video communication, and real-time messaging into a single workspace, allowing users to conduct technical interviews, solve coding problems together, and communicate during interview sessions.

The project focuses on creating an environment where interviewers and candidates can interact through a shared coding workspace while communicating in real time.

---

## ✨ Features

### 💻 Collaborative Code Editor

- VS Code-like coding experience
- Powered by Monaco Editor
- Syntax highlighting
- Support for multiple programming languages
- Real-time collaborative coding

### 📹 Video & Audio Communication

- Real-time video conferencing
- Audio communication
- Designed for interviewer-candidate interaction
- Powered by Stream SDK

### 💬 Real-Time Chat

- Instant messaging
- Communication during interview sessions
- Useful for sharing resources and discussing problems

### 🔐 Authentication

- Secure user authentication
- Session management
- Authentication powered by Clerk

### 🎨 Modern User Interface

- Responsive interface
- TailwindCSS
- DaisyUI
- Modern component-based React architecture

### ⚡ Background Processing

- Asynchronous background tasks
- Event-driven workflows
- Powered by Inngest

---

# 🏗️ System Architecture

The application follows a client-server architecture consisting of:

```text
                ┌─────────────────────┐
                │      Frontend       │
                │   React + Vite      │
                └──────────┬──────────┘
                           │
                           │ HTTP / API
                           ▼
                ┌─────────────────────┐
                │       Backend       │
                │ Node.js + Express   │
                └──────────┬──────────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
        ┌─────────┐   ┌──────────┐  ┌──────────┐
        │ MongoDB │   │  Clerk   │  │ Stream   │
        │ Database│   │   Auth   │  │   SDK    │
        └─────────┘   └──────────┘  └──────────┘
