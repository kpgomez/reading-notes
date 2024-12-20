# Django API steps

## Initial Project Setup

| Step | Description | Environment | Command |
| ---- | ----------- | ----------- | ------- |
| 1 | Create new directory | Terminal | `mkdir <new_directory>` |
| 2 | Step into new directory |Terminal | `cd <new_directory>` |
| 3 | Create virtual environment | Terminal | `python3.11 -m venv .venv` |
| 4 | Activate virtual environment |Terminal | `source .venv/bin/activate` |
| 5 | Install all dependencies | Terminal | `pip install <library>` |
| 6 |Pip freeze|Terminal | `pip freeze > requirements.txt` |
| 7 | Create essential repo file | Terminal | `touch README.md`|
| 8 | Create essential repo file | Terminal | `touch .gitignore`|
| 9 | Create essential docker file | Terminal | `touch Dockerfile`|
| 10 |Create essential docker file | Terminal | `touch docker-compose.yml`|
| 11 |Initialize as git repo | Terminal | `git init` |
| 12 |Connect to remote repo | Terminal | `git remote add origin <https://github.com/{username}/{repo_name}.git_>` |
| 13 | Push to remote repo | Terminal | `git status` |
| ... | ... | ... | `git add .`|
| ... | ... | ... | `git commit -m "initial project setup" .` |
| ... | ... | ... | `git push origin main` |
| 14 | Create new Django project | Terminal | see Django command a |
| 15 | Create new Django app(s) | Terminal | see Django command b |


| 16 | Create a urls.py for each app | Terminal | `touch <app_name>/urls.py` |
| 17 | Add each custom app to settings.py | IDE | n/a |
| 18 | Add each third-party app to settings.py | IDE | n/a |
| 19 | Create new custom user models as per best practices | IDE | n/a |
| 20 | Create new user forms | IDE | n/a |
| 21 | Update admin.py | | |


## Next steps

### Create urls.py in the directory of each custom app

### Add custom app(s) and/or any third-party apps to INSTALLED_APPS in Settings.py

```python

INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",

    # third-party

    # custom apps
]
```
## Custom User Models
** consider drawing UML diagram prior to creating the models **
### 1. Create Custom User Models
[see previous notes](/code-401/class-29.md)

```python
# custom_app/models.py
from django.contrib.auth.models import AbstractUser
from django.db import models

class CustomUser(AbstractUser):
    pass
    # add additional fields in here

    def __str__(self):
        return self.username
```

### 2. Create forms.py and update forms

```python
# custom_app/forms.py
from django.contrib.auth.forms import UserCreationForm, UserChangeForm

from .models import CustomUser

class CustomUserCreationForm(UserCreationForm):

    class Meta:
        model = CustomUser
        fields = ("username", "email")

class CustomUserChangeForm(UserChangeForm):

    class Meta:
        model = CustomUser
        fields = ("username", "email")
```

### 3. Update admin.py

```python
# accounts/admin.py
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin

from .forms import CustomUserCreationForm, CustomUserChangeForm
from .models import CustomUser

class CustomUserAdmin(UserAdmin):
    add_form = CustomUserCreationForm
    form = CustomUserChangeForm
    model = CustomUser
    list_display = ["email", "username",]

admin.site.register(CustomUser, CustomUserAdmin)
```

## Django Commands

| Reference | Command | Description | Notes |
| - | - | - | - |
| a | `django-admin startproject <project_name_project> .` | create new Django project | creates a django project package which includes asgi.py, settings.py,  urls.py, wsgi.py |
| b | `python manage.py startapp <app_name>` | create new Django app|each django app includes a migrations package, admin.py, apps.py, models.py, tests.py, views.py | ... |


## Libraries

| Name | Description | Command | Import Statement | Documentation |
| - | - | - | - | - |
| Django | Batteries included web development framework | `pip install django` | ... |...|
| Django-Cors-Headers | ... | `pip install django-cors-headers` | ... | [documentation](https://pypi.org/project/django-cors-headers/) |
| Django-Environ | ... | `pip install django-environ` | ... | ... |
| Django REST Framework | ... | `pip install djangorestframework` | ... | ... |
| Django REST Framework Simple JWT | ... | `pip install djangorestframework-simplejwt` | ... | ... |
| Gunicorn | Production grade server application | `pip install gunicorn` | ... | ... |
| MultiSelectField| ... |`pip install django-multiselectfield` | `from multiselectfield` | [documentation](https://pypi.org/project/django-multiselectfield/) |
| Psycopgbinary-2 | Postgres Adapter | `pip install psycopg2-binary` | ... | ... |
| Tailwind CSS | Utility First Custom CSS Library | `npm install -D tailwindcss` | ... | ... |
| Whitenoise | ... | `pip install whitenoise` | ... | ... |

## Tailwind
- [Documentation](https://tailwindcss.com/docs/installation)

## README templates
- [How to Write a Good README file (FreeCodeCamp)](https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/)

### Code Challenges
```markdown
# Challenge Title
<!-- Description of the challenge -->

## Whiteboard Process
<!-- Embedded whiteboard image -->

## Approach & Efficiency
<!-- What approach did you take? Why? What is the Big O space/time for this approach? -->

## Solution
<!-- Show how to run your code, and examples of it in action -->
```

### Labs

```markdown
# LAB - Class xx
## Project: Project Name Here
### Author: Student/Group Name
### Links and Resources
- back-end server url (when applicable)
- front-end application (when applicable)

### Setup
.env requirements (where applicable)
i.e.

- PORT - Port Number
- DATABASE_URL - URL to the running Postgres instance/db

#### How to initialize/run your application (where applicable)
- e.g. python main.py

#### How to use your library (where applicable)

#### Tests
- How do you run tests?
- Any tests of note?
- Describe any tests that you did not complete, skipped, etc
```

### Group Projects

### Personal Projects
#### Starter Template
```markdown

# Inspiration
# Description
# Lessons Learned
# Sources/Attribution

```

### Github Profile

## Other Templates
- [gitignore example](https://github.com/kpgomez/drf-auth/blob/main/.gitignore)
- [Dockerfile example](https://github.com/kpgomez/drf-auth/blob/main/Dockerfile)
- [docker-compose.yml](https://github.com/kpgomez/drf-auth/blob/main/docker-compose.yml)
