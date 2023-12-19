# Class 29

## Sources
- [Reading: Django Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)
- [Reading: DjangoX](https://github.com/wsvincent/djangox)
- [Video: Creating a Custom User Model](https://www.youtube.com/watch?v=eCeRC7E8Z7Y&t=59s)
- [Video: Abstract User, User Profile, and Signals in Django](https://www.youtube.com/watch?v=EudKs1HPUfE)

## Bookmark and Review
- [Substituting a custom User model](https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#auth-custom-user)

## Reading Questions
[ChatGPT Summary](https://chat.openai.com/c/d660b63a-3d57-4bfe-9554-89404f5afd91)
1. What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?
> According to ChatGPT, the key benefits include flexibility in user fields, improved authentication, enhanced security, easier integration with third-party apps, better scalability and maintenance, and better consistency across projects. You can define your own user fields, choose any field for authentication purposes such as email as primary identifier for authentication, more control over structure and behavior, easier to modify models without significant application restructuring.  
2. Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.
> Here are the steps to create and implement a Custom User Model after both the project and app have been created. Special note to skip migration step until after the custom model is implemeneted.  Step one, add name_of_new_app to INSTALLED_APPS in settings.py. Step two, change AUTH_USER_MODEL to "name_of_new_app.CustomUser" also in settings.py. Step three, create new User Model in models.py

```python
from django.contrib.auth.models import AbstractUser
from django.db import models

# custom user manager class
    # create user
    # create super user

# custom user object
class CustomUser(AbstractUser):
    # all custom user fields
    # all required user fields that are part of the AbstractUser class

    USERNAME_FIELD = "login_field"
    REQUIRED_FIELDS = ["field1", "field2", "etc"]
    
    objects = "customer_user_manager"
    def __init__(self):
        return self.username
    
    # all required functions
```
> Last step, run `python manage.py makemigrations` then run `python manage.py migrate` to apply models.

3. What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project 

[DjangoX](https://wsvincent.com/djangox-new-starter-framework/)
> DjangoX is a batteries-included Django starter project. It extends the default Django framework with a pre-defined email/password authentication, and can also be authenticated with the user's social media account such as Gmail, Facebook, etc. A use case would be if you wanted a starter project that already has email/password or social authentication so you don't have to build that yourself.