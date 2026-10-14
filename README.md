# Basic Django Project

A simple Django blog and contact web application built step-by-step.

## Tech Stack

- Python 3.x
- Django 4.2+
- SQLite (default)
- Bootstrap 5

## Setup

```bash
# 1. Clone the repo
git clone https://github.com/your-username/Basic-Django-Project-main.git
cd Basic-Django-Project-main

# 2. Create and activate a virtual environment
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # macOS/Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Apply database migrations
cd Hello
python manage.py migrate

# 5. Create a superuser (for admin panel)
python manage.py createsuperuser

# 6. Run the development server
python manage.py runserver
```

## URLs

| URL           | Description                  |
| ------------- | ---------------------------- |
| `/`           | Redirects to blog list       |
| `/blog/`      | List of all blog posts       |
| `/blog/<id>/` | Detail view of a single post |
| `/contact/`   | Contact form                 |
| `/admin/`     | Django admin panel           |

## Features

- Blog posts with title, content, author, and publish date
- Detail page for each post
- Contact form that stores messages in the database
- Bootstrap 5 responsive UI
- Django admin for content management

## Project Structure

```
Basic-Django-Project-main/
├── Hello/
│   ├── Hello/          # Project config (settings, urls, wsgi)
│   ├── blog/           # Blog app (models, views, templates)
│   └── manage.py
├── .gitignore
├── requirements.txt
└── README.md
```
