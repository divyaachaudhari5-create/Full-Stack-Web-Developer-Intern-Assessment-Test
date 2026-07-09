# Full-Stack Startup Space Web Application

A responsive, secure, full-stack web application built for a fictional startup company to handle customer enquiries. This project includes a client-facing corporate website, data validation, automated relational storage, and a robust, authenticated Admin Dashboard with search and filter mechanics.

## 🚀 Features Implemented

- **Responsive Frontend:** 5-page corporate ecosystem (Home, About, Services, Contact, Admin Dashboard) built utilizing highly responsive UI design layouts.
- **Data Validation & Persistence:** Contact form equipped with input validation constraints, providing instant visual feedback on submission success or failure.
- **RESTful Architecture:** Structural views routing `POST` requests from the client to the persistence layer, paired with full CRUD controls inside the admin interface.
- **Robust Admin Dashboard:** A fully protected administrative space featuring live searching, filtering by date/status, and inline status updates (`Pending` vs `Resolved`).
- **Secure Authentication:** Password-hashing and session-based protection mechanism restricting access to unauthorized visitors.

---

## 🛠️ Technology Stack Used

- **Frontend:** HTML5, Tailwind CSS (via Content Delivery Network)
- **Backend Framework:** Python / Django 
- **Database Layer:** SQLite3 (Relational Database)
- **Security Protocols:** Django Authentication Middleware & CSRF Tokens

---

## 📂 Project Architecture

```text
fictional_company/
│
├── fictional_company/          # Core Project Configurations
│   ├── __init__.py
│   ├── settings.py             # App registration and system properties
│   └── urls.py                 # Global application URL routing
│
├── core/                       # Main Functional Application Module
│   ├── templates/              # UI Architecture
│   │   ├── base.html           # Master Layout & Navigation Layout
│   │   ├── home.html           
│   │   ├── about.html
│   │   ├── services.html
│   │   ├── contact.html        # Form Component with CSRF safety
│   ├── admin.py                # Admin Dashboard CRUD controls configuration
│   ├── models.py               # Database Schema definition
│   └── views.py                # Business logic & form handling controllers
│
└── manage.py                   # Administrative execution script
