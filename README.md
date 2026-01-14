# Online Examination System (Django)

The **Online Examination System** is a Django-based web application designed to manage online exams with a role-based architecture. The system provides three dedicated panels: **Admin**, **Teacher**, and **Student**, enabling secure and efficient examination management for educational institutions.

---

## Features

* Role-based authentication (Admin, Teacher, Student)
* Exam creation and management
* Question bank handling
* Online exam attempts with time limits
* Automatic result generation
* Secure login and access control

---

## Technology Stack

* **Backend:** Django, Django REST Framework
* **Frontend:** HTML, CSS, Bootstrap, JavaScript
* **Database:** SQLite (default)
* **Language:** Python 3.x

---

## Project Setup & Run Instructions

Follow the steps below to run this project on your local machine.

---

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Online-Examination-System.git
cd Online-Examination-System
```

---

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

---

### 3. Install Dependencies

Make sure `requirements.txt` exists, then run:

```bash
pip install -r requirements.txt
```

If `requirements.txt` does not exist, generate it using:

```bash
pip freeze > requirements.txt
```

---

### 4. Apply Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

---

### 5. Create Superuser (Admin)

```bash
python manage.py createsuperuser
```

Provide username, email, and password when prompted.

---

### 6. Run the Development Server

```bash
python manage.py runserver
```

Open your browser and visit:

```
http://127.0.0.1:8000/
```

Admin Panel:

```
http://127.0.0.1:8000/admin/
```

---

## User Roles

* **Admin:** Full system control and user management
* **Teacher:** Exam and question management
* **Student:** Exam participation and result viewing

---

## Folder Structure (Simplified)

```
Online-Examination-System/
│
├── exam/
├── student/
├── teacher/
├── templates/
├── static/
├── venv/
├── db.sqlite3
├── manage.py
├── requirements.txt
└── README.md
```

---
