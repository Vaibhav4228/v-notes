# V-Notes 🗒️ – Secure Full Stack Notes Management System

Welcome to **V-Notes**, a production-ready full-stack application built to showcase mastery of **Spring Security**, **OAuth2**, **MFA**, and **ReactJS**. This project is more than just a note-taking app – it's a **secure**, **scalable**, and **auditable** system that demonstrates real-world security implementations.

> 🔐 Master Spring Security with React JS by building a secure notes application.

## 🌐 Live Frontend URL
[https://v-notes-iota.vercel.app/](https://v-notes-iota.vercel.app/)

## 🐳 Docker Backend Image
```bash
docker pull vaibhav990/v-notes
```

---

## 🔥 Key Features

### ✅ Authentication & Authorization
- Secure user signup/login with **Spring Security**
- Integration with **OAuth2.0** (Google & GitHub login)
- **JWT** token-based authentication
- **CSRF** protection
- **MFA (Multi-Factor Authentication)** using authenticator apps like Google Authenticator

### 🛡️ Password & Session Management
- Password reset via email link with unique tokenized URLs
- Login session control & user state management (locked, enabled, expired)
- View current username & user details via secure endpoints

### 🗒️ Notes Functionality
- Authenticated users can create, update, delete, and view notes
- Notes are stored securely and associated with user identities

### 🧑‍💼 Admin Panel
- Admin users can:
  - View complete user list
  - View audit logs for user activities
  - Update user roles and status (locked, expired, enabled, credentials expired)
  - Fetch individual user data and role-based info

---

## 📑 Swagger API Overview

### 📓 Note Controller
- `GET /api/notes`
- `POST /api/notes`
- `PUT /api/notes/{noteId}`
- `DELETE /api/notes/{noteId}`

### 🔐 Auth Controller
- `POST /api/auth/public/signup`
- `POST /api/auth/public/signin`
- `POST /api/auth/public/forgot-password`
- `POST /api/auth/public/reset-password`
- `POST /api/auth/verify-2fa`
- `POST /api/auth/public/verify-2fa-login`
- `POST /api/auth/enable-2fa`
- `POST /api/auth/disable-2fa`
- `GET /api/auth/user`
- `GET /api/auth/user/2fa-status`
- `GET /api/auth/username`

### ⚙️ Admin Controller
- `GET /api/admin/getusers`
- `GET /api/admin/user/{id}`
- `GET /api/admin/roles`
- `PUT /api/admin/update-role`
- `PUT /api/admin/update-password`
- `PUT /api/admin/update-lock-status`
- `PUT /api/admin/update-expiry-status`
- `PUT /api/admin/update-enabled-status`
- `PUT /api/admin/update-credentials-expiry-status`

### 📊 Audit Log Controller
- `GET /api/audit`
- `GET /api/audit/note/{id}`

### 🌐 Miscellaneous
- `GET /api/csrf-token`
- `GET /hi`
- `GET /hello`
- `GET /contact`

---

## 📦 Tech Stack

### 🧩 Backend
- Java 17
- Spring Boot 3
- Spring Security + JWT + OAuth2.0
- PostgreSQL (or any preferred DB)
- Dockerized deployment

### 💻 Frontend
- React.js (Vite)
- Tailwind CSS for styling
- Axios for API integration

### 🔐 Security
- JWT Authentication
- OAuth2.0 (Google, GitHub)
- Multi-Factor Authentication (MFA)
- CSRF protection

---

## 📂 Project Structure

```bash
├── backend
│   └── src/main/java/com/vnotes/...
├── frontend
│   └── src/components/...
├── docker-compose.yml
└── README.md
```

---

## 🚀 Get Started

### Backend (Docker)
```bash
docker pull vaibhav990/v-notes
docker run -p 8080:8080 vaibhav990/v-notes
```

### Frontend (Vercel)
Visit: [https://v-notes-iota.vercel.app/](https://v-notes-iota.vercel.app/)

---

## 👨‍💻 Developed By

**Vaibhav Sharma**  
🔗 [GitHub](https://github.com/Vaibhav4228) | [LeetCode](https://leetcode.com/u/vaibhav990/) | [Instagram](https://www.instagram.com/vaibhav_sharmatic9?igsh=dXA4aGNvcmJyMW56)

---

## 📜 License
This project is licensed under the MIT License.