# Blog & Content Management System (Django + MySQL)

A starter Blog & Content Management System built with Django and configured for MySQL.

## Features
- User registration / login / logout
- Author profiles
- Category-based blog posts
- Draft / Published status
- CRUD for blog posts
- Comments on posts
- Search posts
- My posts page
- Admin panel support

## Setup

```bash
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Linux/Mac

pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## MySQL Configuration
Update database credentials in:
`blog_cms/settings.py`

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'blog_cms_db',
        'USER': 'root',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

## Default URLs
- Home: `/`
- Register: `/accounts/register/`
- Login: `/accounts/login/`
- Posts: `/posts/`
- My Posts: `/posts/my/`
- Admin: `/admin/`
