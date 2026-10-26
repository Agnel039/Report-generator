<div align="center">

# 📊 Report-generator

**A Django project to generate reports — set up and running in minutes.**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-Framework-092E20?style=for-the-badge&logo=django&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Development-orange?style=for-the-badge)

</div>

---

## 📑 Table of Contents

- [Prerequisites](#-prerequisites)
- [Quick Start](#-quick-start)
- [Detailed Setup](#-detailed-setup)
- [Project Structure](#-project-structure)
- [Useful Commands](#-useful-commands)

---

## ✅ Prerequisites

Make sure you have the following installed:

- [Python 3.x](https://www.python.org/downloads/)
- `pip` (comes with Python)

---

## ⚡ Quick Start

```bash
mkdir Report-generator
cd Report-generator
python -m venv venv
.\venv\Scripts\activate
python -m pip install django
django-admin startproject config .
python manage.py migrate
python manage.py runserver
```

Then open 👉 **http://127.0.0.1:8000/**

---

## 🛠️ Detailed Setup

### Step 1 — Create the project folder

```bash
mkdir Report-generator
cd Report-generator
```

### Step 2 — Set up a virtual environment

**2.1 Create the venv**

```bash
python -m venv venv
```

**2.2 Activate the venv**

| OS | Command |
|----|---------|
| 🪟 Windows (PowerShell / CMD) | `.\venv\Scripts\activate` |
| 🍎 macOS / 🐧 Linux | `source venv/bin/activate` |

> 💡 You'll know it worked when `(venv)` appears at the start of your terminal prompt.

### Step 3 — Install Django

**3.1 Install**

```bash
python -m pip install django
```

**3.2 Confirm the installation**

```bash
django-admin --version
```

### Step 4 — Create the Django project

```bash
django-admin startproject config .
```

> 📌 The trailing `.` creates the project in the current folder instead of nesting it in a new one.

### Step 5 — Run database migrations

```bash
python manage.py migrate
```

### Step 6 — Start the development server

```bash
python manage.py runserver
```

🎉 Visit **http://127.0.0.1:8000/** — you should see the Django welcome page.

---

## 🧩 Optional: Create an App

If your project needs multiple apps, create one like this:

```bash
python manage.py startapp core
```

Then register it in `config/settings.py`:

```python
INSTALLED_APPS = [
    # ...
    "core",
]
```

---

## 📁 Project Structure

```text
Report-generator/
├── venv/               # Virtual environment
├── config/             # Project settings
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
├── core/               # Optional app
├── db.sqlite3          # Created after migrate
└── manage.py           # Django command-line utility
```

---

## 🧰 Useful Commands

| Purpose | Command |
|---------|---------|
| Run the server | `python manage.py runserver` |
| Create an app | `python manage.py startapp <name>` |
| Make migrations | `python manage.py makemigrations` |
| Apply migrations | `python manage.py migrate` |
| Create an admin user | `python manage.py createsuperuser` |
| Deactivate the venv | `deactivate` |

---

<div align="center">

Made with ❤️ using Django

</div>