# jobnet
🚀 JobNet — мини-соцсеть для управления проектами и командной работы 👨‍💻👩‍🚀
# 🌐 JobNet — Social Task Network for Team Collaboration

**JobNet** is a social-style task management web application for organizing and planning team-based projects. Built with Flask and SQLAlchemy, it allows users to collaborate, distribute responsibilities, and manage tasks across different departments in a secure, structured way.

## 🎯 Purpose

JobNet simulates the core of a **social intranet platform** where users register, create and assign tasks (jobs), manage work by departments, and control access — ideal for internal project management in small to medium teams.

## 🚀 Features

- 👤 **User Accounts** — registration, login, session management
- 👥 **User Profiles** — see who created what
- 💼 **Jobs (Tasks)** — add, edit, delete tasks with access control
- 🏢 **Departments** — group work by teams/sections
- 🏷 **Job Categories** — organize jobs via many-to-many relationship
- 🔐 **Permissions**:
  - Only authors or the admin (`user.id == 1`) can edit/delete jobs
  - Only logged-in users can create new jobs or departments
- 📄 **Template-Based UI** using Jinja2 and base layout inheritance
- 💾 **Security**:
  - Password hashing
  - Role-based access (admin, team leader)
  - Session control with Flask-Login

## 🧱 Technologies Used

- Python 3.10+
- Flask
- SQLAlchemy
- Flask-WTF (Forms)
- Flask-Login
- Jinja2 Templating
- HTML/CSS (Bootstrap-friendly layout)

## 📂 Folder Structure

jobnet/
├── static/ # CSS, JS
├── templates/ # HTML templates
│ ├── base.html
│ ├── login.html
│ ├── register.html
│ ├── jobs.html
│ └── ...
├── models/ # SQLAlchemy models
├── forms/ # WTForms forms
├── main.py # App logic and routes
├── config.py # Flask config
└── db/ # SQLite DB and migration scripts
