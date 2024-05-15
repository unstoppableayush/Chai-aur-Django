# Django Series

## Start a Django project and file structure

- It is Rapid development framework.
- `uv` - An extremely fast Python package installer and resolver, written in Rust.
- It is faster, more efficient, and easier to use.
- installation - `pip install uv`
- It is Python package manager.
- Crated a virtual enviornment
    -  `uv venv`
    - acitvate - `venv\Scripts\activate`
    - deactivate - `deactivate`

- Install Django - `uv pip install Django`
- Install Project - `django-admin startproject ChaiaurDjango`
- Running Project - `python manage.py runserver `
- Running Project on specific port - `python manage.py runserver 8001`
- Learned about file structure in Django.


## Jinja Templates and Errors in Django

**Architecture in Djnago**
---

USER -> Django -> URL Resolver -> `url.py` -> (url.py, url.py ...) -> views.py (main controller , logic) <-> Model.py -> DB

Django <-  Response <- Views.py

Django <- Templates- <-  Response <- Views.py

- Created views `home, about, contact` and returning `HttpResponse`

- learned about how to use template folder
- directory structure inside template
- load static content using `common template tag`
- Told the file using `{% load static %}`  that i'm going to load static file.
- imported the os library in `setting.py`
- used `STATICFILES_DIRS = [os.path.join(BASE_DIR, 'static')]` to load static assets.

ASSIGNMENT
---
To render web pages for about us and contact s page using static files.