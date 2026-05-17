# ✅ Django Advanced To-Do List App

A modern productivity and task management web application built with **Django**, **SQLite**, and **Tailwind CSS**.

This project started as a simple CRUD To-Do app and was upgraded into a fully authenticated productivity system with:

- 🔐 User Authentication
- 🏷️ Categories
- ⚡ Priorities
- 📅 Due Dates
- 🔍 Search & Filters
- 🎨 Responsive Tailwind UI
- ⚙️ Django Admin Integration

---

# 📸 Application Screenshots

---

## 🔐 Login Page

![Login Page](images/Login%20Page.png)

---

## 🏠 Home Page

![Home Page](images/Home%20Page.png)

---

## 📝 Create New Task

![Create New Task](images/Create%20New%20Task.png)

---

## ✏️ Update Task #1

![Update Task #1](images/Update%20Task%20%231.png)

---

## 🗑️ Delete Task

![Delete Task](images/Delete%20Task.png)

---

## 🏷️ Create Category

![Create Category](images/Create%20Category.png)

---

## ✅ Toggle Complete Task

![Toggle Complete Task](Assesst\Toggle Complete Task.png)

---

# 🚀 Features

## ✅ Core Features

- Create tasks
- Edit tasks
- Delete tasks
- Toggle completed tasks
- Responsive UI
- Animated task cards

---

# 🔐 Authentication

- User login/logout
- User-specific tasks
- Protected routes using `@login_required`
- Secure logout using POST requests

---

# 🏷️ Categories

Users can:

- Create categories
- Assign categories to tasks
- Filter tasks by category

Examples:
- Work
- Personal
- Shopping
- School

---

# ⚡ Priority Levels

Tasks support:

- Low Priority
- Medium Priority
- High Priority

With color-coded badges.

---

# 📅 Due Dates

Features include:

- Due dates
- Overdue detection
- Today's tasks
- Upcoming tasks

---

# 🔍 Search & Filtering

Users can filter by:

- Status
- Priority
- Category
- Due date
- Search keywords

Search supports:
- Task title
- Task description

---

# 🎨 UI / UX Features

Built using Tailwind CSS with:

- Gradient animated background
- Responsive layouts
- Hover animations
- Card-based UI
- Modern form styling
- Clean dashboard layout

---

# 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Django | Backend Framework |
| SQLite | Database |
| Tailwind CSS | Styling |
| HTML | Templates |
| JavaScript | Client-side interactions |

---

# 📂 Project Structure

```text
todoproject/
│
├── images/
│   ├── Login Page.png
│   ├── Home Page.png
│   ├── Create New Task.png
│   ├── Update Task #1.png
│   ├── Delete Task.png
│   ├── Create Category.png
│   └── Toggle Complete Task.png
│
├── manage.py
├── db.sqlite3
│
├── todoproject/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
├── todos/
│   ├── migrations/
│   ├── templates/
│   │   └── todos/
│   │       ├── base.html
│   │       ├── login.html
│   │       ├── todo_list.html
│   │       ├── todo_form.html
│   │       ├── todo_confirm_delete.html
│   │       └── category_form.html
│   │
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone <your-repository-url>
cd todoproject
```

---

## 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install django
```

---

## 4️⃣ Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

---

## 5️⃣ Create Superuser

```bash
python manage.py createsuperuser
```

---

## 6️⃣ Run Development Server

```bash
python manage.py runserver
```

---

# 🌐 Application URLs

## Main App

```text
http://127.0.0.1:8000/
```

## Login Page

```text
http://127.0.0.1:8000/login/
```

## Create Task

```text
http://127.0.0.1:8000/create/
```

## Create Category

```text
http://127.0.0.1:8000/category/create/
```

## Admin Panel

```text
http://127.0.0.1:8000/admin/
```

---

# 📋 Full URL Map

| Page | URL |
|---|---|
| Home | `/` |
| Login | `/login/` |
| Logout | `/logout/` |
| Create Task | `/create/` |
| Update Task | `/<id>/update/` |
| Delete Task | `/<id>/delete/` |
| Toggle Task | `/<id>/toggle/` |
| Create Category | `/category/create/` |
| Admin Panel | `/admin/` |

---

# 🔍 Filter Examples

## Search

```text
/?q=meeting
```

## Completed Tasks

```text
/?status=completed
```

## Pending Tasks

```text
/?status=pending
```

## High Priority Tasks

```text
/?priority=high
```

## Today's Tasks

```text
/?due=today
```

## Combined Filters

```text
/?q=report&status=pending&priority=high
```

---

# 🧠 Database Models

## Todo Model

Fields:
- title
- description
- completed
- priority
- due_date
- category
- owner
- created_at
- updated_at

---

## Category Model

Fields:
- name
- owner

---

# 🔒 Security Features

- CSRF protection
- User-specific query filtering
- Protected routes
- Secure logout using POST requests

---

# 🐛 Common Issues

## `TemplateDoesNotExist`

Ensure templates are located inside:

```text
todos/templates/todos/
```

---

## Migrations Not Detected

Ensure this file exists:

```text
todos/migrations/__init__.py
```

---

## `IntegrityError: owner`

Delete `db.sqlite3` and rerun migrations during development.

---

# 🚀 Future Improvements

Potential upgrades:

- Dark mode
- AJAX interactions
- Drag & drop tasks
- REST API
- React frontend
- AI assistant
- Notifications
- Calendar integration
- Pomodoro timer

---

# 📚 Learning Outcomes

This project demonstrates:

- Django models
- CRUD operations
- Authentication
- Form handling
- Query filtering
- Template inheritance
- Database migrations
- Tailwind UI development
- User authorization

---

# 👩‍💻 Author

Created by Hala Korayem

---

# 📄 License

This project is for educational and portfolio purposes.