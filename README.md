# Watchmate

Watchmate is a Django-based web application for managing and tracking your watchlist of movies, TV shows, or other items. This project demonstrates a simple Django setup with a custom app (`watchlist_app`).

## Features
- Add, view, and manage items in your watchlist
- Django admin integration
- SQLite database for development

## Project Structure
```
watchmate/
├── db.sqlite3
├── manage.py
├── watchlist_app/
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── migrations/
├── watchmate/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── menv/ (virtual environment)
```

## Setup Instructions

1. **Clone the repository** (if applicable):
   ```powershell
   git clone <repo-url>
   cd watchmate
   ```

2. **Create and activate a virtual environment** (if not already present):
   ```powershell
   python -m venv menv
   .\menv\Scripts\Activate.ps1
   ```

3. **Install dependencies:**
   ```powershell
   pip install django
   ```

4. **Apply migrations:**
   ```powershell
   python manage.py migrate
   ```

5. **Create a superuser (for admin access):**
   ```powershell
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```powershell
   python manage.py runserver
   ```

7. **Access the app:**
   - Open your browser and go to `http://127.0.0.1:8000/`
   - Admin interface: `http://127.0.0.1:8000/admin/`

## App Details
- **App Name:** `watchlist_app`
- **Main files:** `models.py`, `views.py`, `urls.py`, `admin.py`
- **Database:** SQLite (default for Django projects)

## License
This project is for educational purposes.
