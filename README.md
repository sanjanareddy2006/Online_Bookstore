 📚 Django Online Bookstore Project

A complete **Online Bookstore Web Application** built using Django. This project allows users to browse books, view detailed information, add them to a shopping cart, and view basic analytics. It includes dynamic page rendering using Django Templates and an admin panel for backend book management.

 🚀 Features

- 📖 Home page with book listings
- 📘 Book detail page
- 🛒 Shopping cart functionality
- 📊 Analytics dashboard
- 🧑‍💼 Django Admin panel
- 📷 Image upload and media file handling
- 🎨 Custom CSS for styling
- ✅ SQLite3 for database

 🛠️ Tech Stack

- Backend: Python, Django
- Frontend: HTML, CSS (Templates & Static files)
- Database: SQLite3
- Media: Django media configuration
- Others: Django Admin, Django ORM


 📂 Project Structure

OnlineBookstore/
│
├── bookstore/                 # Django App
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── tests.py
│   ├── migrations/
│   └── media/books/
│       └── pythonimg.jpg
│
├── OnlineBookstore/          # Project Settings
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
├── templates/                # HTML Templates
│   ├── base.html
│   ├── index.html
│   ├── book_detail.html
│   ├── cart.html
│   └── analytics.html
│
├── static/                   # CSS
│   └── styles.css
│
├── db.sqlite3                # Database
├── manage.py                 # Django manager
├── requirements.txt          # Project dependencies
└── projectKFR.txt            # Report / Summary
```

 ✅ How to Run the Project

 1. Clone the Repository

```bash
git clone https://github.com/yourusername/online-bookstore.git
cd online-bookstore
```
 2. Create a Virtual Environment

```bash
python -m venv venv
# Activate the environment
venv\Scripts\activate      # For Windows
source venv/bin/activate     # For macOS/Linux
```

 3. Install Dependencies

```bash
pip install -r requirements.txt
```

 4. Apply Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

 5. Create Superuser (Optional)

```bash
python manage.py createsuperuser
```
 6. Run the Server

```bash
python manage.py runserver
```

Visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

 🖼️ Media Handling

In `settings.py`, make sure the following lines exist:

```python
MEDIA_URL = '/media/'
MEDIA_ROOT = BASE_DIR / 'media'
```

In `urls.py` of your main project folder:

```python
from django.conf import settings
from django.conf.urls.static import static

urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
```

---

 📸 Template Pages Overview

| Template        | Purpose                          |
|----------------|----------------------------------|
| `index.html`        | Home page with all books       |
| `book_detail.html`  | Individual book detail page    |
| `cart.html`         | Shopping cart view             |
| `analytics.html`    | Analytics/dashboard view       |
| `base.html`         | Common template layout         |

---

 🧾 Sample `requirements.txt`

```
Django>=4.0,<5.0
```

Generate yours by:

```bash
pip freeze > requirements.txt
```

---

👤 Author

Developed by **[Sripathi Sanjana Reddy]**


