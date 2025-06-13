
# 🌟 Virtual Community Support – Full Stack Web Application

A robust and dynamic platform that enables users to discover, apply for, and manage social missions. Designed with both users and admins in mind, this full-stack project blends powerful technologies into a clean, secure, and scalable solution.

---

## 🌐 Overview

**Virtual Community Support** is an end-to-end web application that helps communities connect with volunteering missions.  
It supports user registration, secure login, mission discovery with filters, and application management.  
Admins have complete control over mission listings, themes, users, and role-based authorization.

> This project was developed using modern web technologies like Angular, ASP.NET Core, and PostgreSQL following clean architecture principles.

---

## 🚀 Core Features

### 👤 User Side
- 🔐 JWT-based secure authentication  
- 🔍 Filter & explore missions by theme, skill, or location  
- 📝 Apply to missions and view application history  
- 👤 Edit personal profile, upload image  

### 🛠️ Admin Side
- 🧾 Full CRUD on missions, themes, skills  
- 👥 Manage user roles and applications  
- 🛡️ Role-based access for Admin & User  
- 📊 Admin dashboard for quick insights  

---

## 🧠 Tech Stack

### 🔹 Frontend
- Angular 14+  
- Bootstrap, Angular Forms, Reactive Forms  
- RxJS, ngx-pagination, ngx-toastr  

### 🔹 Backend
- ASP.NET Core Web API  
- Entity Framework Core (Code First)  
- PostgreSQL  
- Swagger for API Documentation  
- JWT Authentication & Authorization  

---

## 📁 Project Folder Structure

```
📁 Project-mission  
├── 📂 Mission-frontend (Angular)  
│   ├── 📂 app  
│   │   ├── 📂 components → Login, Register, Profile, Dashboard  
│   │   ├── 📂 services → API integration, Auth, Missions  
│   │   ├── 📂 modules → AuthModule, AdminModule, UserModule  
│   │   ├── 📂 guards → Route guards for role-based access  
│   │   ├── 📂 interceptors → JWT interceptor for API security  
│   ├── 📂 assets → Images, logos, styles  
│   ├── 📂 environments → Development & production configs  

├── 📂 Mission-backend (ASP.NET Core)  
│   ├── 📂 Controllers → LoginController, MissionController, AdminUserController  
│   ├── 📂 Models → DTOs, Entity Models  
│   ├── 📂 Services → Business logic (MissionService, AuthService, etc.)  
│   ├── 📂 Repositories → DB operations, LINQ queries  
│   ├── 📂 DataContext → EF DbContext & Seeding  
│   ├── 📄 Program.cs → App Entry point  
│   └── 📄 appsettings.json → DB & JWT configuration  
```

---

## 📡 API Endpoints Overview

### 🔐 Authentication & Authorization
- `POST /api/Login` → User login with JWT token  
- `POST /api/Register` → User registration  
- `GET /api/UserDetail` → Get logged-in user details  

### 🎯 Mission Management
- `GET /api/Mission` → List all missions  
- `POST /api/Mission` → Add new mission (Admin only)  
- `PUT /api/Mission/{id}` → Update mission  
- `DELETE /api/Mission/{id}` → Delete mission  

### 🏷️ Mission Theme & Skill
- `GET /api/MissionTheme` → Get all themes  
- `POST /api/MissionTheme` → Add theme (Admin)  
- `GET /api/MissionSkill` → Get all skills  
- `POST /api/MissionSkill` → Add skill (Admin)  

### 📄 Application Management
- `POST /api/MissionApplication` → Apply for a mission  
- `GET /api/MissionApplication/User` → Get applied missions (User)  
- `GET /api/MissionApplication/Admin` → Get all applications (Admin)  
- `PUT /api/MissionApplication/Approve/{id}` → Approve/Reject application  

### 👥 Admin User Management
- `GET /api/AdminUser` → List all users  
- `PUT /api/AdminUser/Role/{id}` → Change user role  
- `DELETE /api/AdminUser/{id}` → Remove user  

---

## ⚙️ Local Setup Instructions

### 🔧 Backend (.NET Core)

```bash
cd Mission-backend
dotnet restore
dotnet ef database update
dotnet run
```

### 🔧 Frontend (Angular)

```bash
cd Mission-frontend
npm install
ng serve

---

## 📘 Use Cases

- Volunteer management for NGOs and non-profits  
- College projects involving social work portals  
- CSR program management tools  
- Hackathons & community event platforms  

---

## 👨‍💻 Developed By

**Kirtan Savani**  
GitHub: [@Kirtansavani03](https://github.com/Kirtansavani03)

---

## 📄 License

This project is developed for **educational and demonstration purposes** only.  
Free to fork and explore for learning.

---

## 🧠 Pro Tip

You can containerize this project using **Docker** and deploy it on **AWS EC2**, **Azure App Service**, or **Heroku** for production use.  
Need help? Feel free to reach out!
