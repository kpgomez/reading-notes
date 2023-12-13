# Class 27: Django Models

## Sources
- [Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- [Django Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)
- [Beginner's Guide to Django Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)

## Bookmark and Review
- [Beginner's Guide to Django Part 2](https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html)

## Reading Questions 
[ChatGPT prompt](https://chat.openai.com/c/d2055f03-7075-4580-8d36-33e3fc63ac30)
1. Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application? 
> Purpose of models is to define the structure of your database tables and the relationships between them using Python code instead of directly through SQL. The Python code is translated by the Django application into the corresponding SQL statements needed to create and define the database tables. 
2. Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?
> It can perform all CRUD operations on model instances. It's customizable, comes with a built-in admin interface to manage models, as well as manage user access and permission settings. 
3. Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?
> Key components are the models, views, templates, URLs, and settings. The workflow begins with a request from the user, URL pattern in the request maps to a view, the view handles the logic and preps the data, and template renders the data received from the view into HTML, and then the HTML response is sent back to the user.
## Things I want to learn more about