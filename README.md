# Django Allauth

This is a Django-based project demonstrating the integration of [`django-allauth`](https://github.com/pennersr/django-allauth) for handling user authentication, registration, email verification, password management, and more using a **custom user model**.

---

## 🚀 Features

- ✅ Email-based login (no username)
- ✅ UUID as primary key
- ✅ Phone number field in user model
- ✅ Soft-deletion support (`is_deleted`)
- ✅ Email verification and password reset via SMTP
- ✅ Fully customized authentication templates using Bootstrap

---

## 📦 Tech Stack

- Django
- Python 3
- SQLite (default)
- django-allauth
- Bootstrap 5

---

## 🛠️ Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/Nivedsunil/django-auth-system.git
cd django-auth-system/src/dj_allauth

# 2. Create and activate virtual environment
# On Windows:
python -m venv venv
venv\Scripts\activate

# On macOS/Linux:
# python3 -m venv venv
# source venv/bin/activate

# 3. Install dependencies
pip install -r ../../req.txt

# 4. Add your email config in .env
# Create a .env file in the root and add:
# EMAIL_HOST_USER=your_email@gmail.com
# EMAIL_HOST_PASSWORD=your_app_password

# 5. Run migrations
python manage.py makemigrations
python manage.py migrate

# 6. Create superuser
python manage.py createsuperuser

# 7. Start the development server
python manage.py runserver

#8. Then visit:
http://127.0.0.1:8000/auth/login/
Log in or register a new account to test allauth features.
