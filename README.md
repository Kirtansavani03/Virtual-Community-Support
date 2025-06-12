🌟 Virtual Community Support

> A full-stack web application to manage and connect users with social service missions.

🌐 Overview

> Virtual Community Support is a robust platform built to enable users to discover, apply for, and track missions based on their skills and interests. Admins can manage missions, themes, users, and applications efficiently using a secured backend.

🚀 Features

⭐ User Side
- 🔐 Secure login with JWT-based authentication
- 👥 Role-based access: User & Admin
- 🔍 View and filter missions by themes, skills, or location
- 📄 Apply to missions and track application history
- 🧑‍💼 Edit and update personal profile

⭐ Admin Side
- 🧾 User management (Create, Read, Update, Delete)
- 🎯 Mission CRUD with skills & themes
- 📦 Application approval and management
- 🔐 Role-based authorization

🛠️ Tech Stack

Frontend: Angular  
Backend: ASP.NET Core Web API  
Database: PostgreSQL  
ORM: Entity Framework Core (Code First)  
Security: JWT Authentication & Authorization  

🧩 Modules

🔹 User Module
- Registration & Login
- Role-based dashboard
- Mission browsing, filtering, and sorting
- Profile editing

🔹 Mission Module
- CRUD operations
- Assign themes and skills
- View by status and date

🔹 Application Module
- Apply to missions
- Admin can approve or reject
- Search/filter applications

🔹 Authorization
- JWT token-based login
- Role-based protected routes

📂 Project Structure

Project-mission/  
├── Mission-frontend/       (Angular App)  
│   ├── Components/  
│   ├── Services/  
│   └── Modules & Routing  
├── Mission-backend/        (.NET Core API)  
│   ├── Controllers/  
│   ├── Models/  
│   ├── Services/  
│   ├── Repositories/  
│   └── DataContext/

⚙️ Installation & Setup

✅ Backend Setup
```
cd Mission-backend
dotnet restore
dotnet ef database update
dotnet run
```

✅ Frontend Setup
```
cd Mission-frontend
npm install
ng serve
```

👨‍💻 Author

Kirtan Savani  
GitHub: [@Kirtansavani03](https://github.com/Kirtansavani03)

📃 License

This project is intended for educational and demonstration purposes only.
