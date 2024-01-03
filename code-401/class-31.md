# Class 31

## Notes

- Docker is a Linux container. 
- A docker image is a snapshot in time of what a project contains. 
- A container is a running instance of the image.
- use a Dockerfile to create custom images
- docker-compose.yml contains container instructions
- order matters in a Dockerfile, put code that won't change often at the top and code that will change towards the bottom
- use `python3.11 -m venv .venv` instead of pipenv

## order of commands
- `cd <intended_directory>`
- `mkdir <name_of_folder> && cd <name_of_folder>`
- `mkdir python3.11 && cd python3.11`
- `touch Dockerfile` <- define the image aka list of requirements needed to build our image

add `FROM python:3.11-alpine` to Dockerfile <- imports a base image

- `docker image build .`
- `touch docker-compose.yml`
- `docker-compose up --build`

```python
# Dockerfile

# Python version
FROM python:3.11-alpine

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set work directory
WORKDIR /<name_of_folder>

# Install dependencies
COPY Pipfile Pipfile.lock /<name_of_folder>/
RUN pip install pipenv && pipenv install --system

# Copy project
COPY . /<name_of_folder>/
```

```python
# docker-compose.yml
version: '3.11'

services:
  web:
    build: .
    command: python /code/manage.py runserver 0.0.0.0:8000
    volumes:
      - .:/<name_of_folder>
    ports:
      - 8000:8000
```

### docker commands
- docker run hello-world
- docker info
- docker image ls
- docker container ls -la shows list of all containers
- docker container ls shows list of running containers

## Sources
- [Beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)
- [Django for APIs](https://djangoforapis.com/library-website-and-api/)

## Bookmark and Review
- [Beginner's Guide to Django REST Framework](https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners)

## Reading Questions
1. What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?
> Key components include a Dockerfile, images, and docker-compose.yml. A container can be easily distributed amongst team members and it ensures everyone on the team is working with the same set-up. 
2. Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.
> - Create new directory `mkdir`. 
> - Create virtual environment `python3.11 -m venv .venv` 
> - Activate ve `source .venv/bin/activate`. 
> - Install Django `pip install django`. 
> - Create new project `django-admin startproject project_name .` 
> - `python manage.py migrate`
> - `python manage.py runserver` to test it then Ctrl+C to stop server
> - Add app `python manage.py startapp name_of_app`
> - Add urls.py file to app directory
> - Add new app to list of INSTALLED_APPS in settings.py

```python
# django_project/settings.py
INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",
    # Local
    "books.apps.BooksConfig",  # this is different... why is this not just "books"?
]
```

> - update models.py

```python
# books/models.py
from django.db import models


class Book(models.Model):
    title = models.CharField(max_length=250)
    subtitle = models.CharField(max_length=250)
    author = models.CharField(max_length=100)
    isbn = models.CharField(max_length=13)

    def __str__(self):
        return self.title
```

> - `python manage.py makemigrations <name_of_app>`
> - `python manage.py migrate`
> - `python manage.py createsuperuser`
> - update admin.py

```python
# books/admin.py
from django.contrib import admin

from .models import Book

admin.site.register(Book)
```

> - update views.py

```python
# books/views.py
from django.views.generic import ListView

from .models import Book


class BookListView(ListView):
    model = Book
    template_name = "book_list.html"
```

> - update project-level urls.py

```python
# django_project/urls.py
from django.contrib import admin
from django.urls import path, include  # new

urlpatterns = [
    path("admin/", admin.site.urls),
    path("", include("books.urls")),  # new
]
```

> - update app-level urls.py

```python
# books/urls.py
from django.urls import path

from .views import BookListView

urlpatterns = [
    path("", BookListView.as_view(), name="home"),
]
```

> - create new *templates* folder within the app directory
> - create new *base.html, list.html* file in templates folder

```python
<!-- books/templates/books/book_list.html -->
<h1>All books</h1>
{% for book in book_list %}
<ul>
  <li>Title: {{ book.title }}</li>
  <li>Subtitle: {{ book.subtitle }}</li>
  <li>Author: {{ book.author }}</li>
  <li>ISBN: {{ book.isbn }}</li>
</ul>
{% endfor %}
```

3. Can you explain the primary differences between Django and Django REST framework? 

[ChatGPT Prompt](https://chat.openai.com/c/a2763cbe-18da-4273-b57c-e2048e20a8af)
> Django is for building a quick client-side web application and Django REST is for building a quick server-side RESTful web APIs. 