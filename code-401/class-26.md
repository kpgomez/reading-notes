# Class 26

## Django Notes
`from django.db import models`
`from django.url import path`
`from . import views`
`from django.shortcuts import render`
`from django import forms`
`from django.contrib.auth.decorators import login_required`
`from django.contrib import admin`
`from django.utils.translation import gettext`

`models.CharField(max_length=XXX, choices=())`
`models.BooleanField(default=True)`
`models.ForeignKey()`

`models.Model`
`forms.Form`
`admin.ModelAdmin`

`forms.CharField()`
`forms.EmailField()`
`forms.BooleanField(required=False)`

`return render(request, '.html', {'key' : key})`
`return render(request, '.html', {'current_user' : request.user})`

{%raw%}
`{%'if'%}{% 'endif' %}` 
`{% for %}{% endfor %}`
`{% blocktrans %}{% endblocktrans%}`
`{% plural %}`
`{% if %}{% trans %}{% endif %}` 
{%endraw%}
`{{}}` 

`admin.site.register(XXX)`
`admin.site.register(XXX, XXX)`

## Tailwind Notes
6 utility classes 
- h-10 is height of 10 units
- px-6 is horizontal padding of 6 units
- font-semibold is font weight
- rounded-md is border radius <- unsure what 'md' is
- bg-black is background and color
- text-white is text color

example `<button class="h-10 px-6 font-semi-bold rounded-md bg-black text-white" type="submit">Buy now</button>`

## Sources
- [Getting Started with Django](https://www.djangoproject.com/start/)
- [How Django Works Behind the Scenes](https://wsvincent.com/how-django-works-behind-the-scenes/)
- [What is Tailwind CSS?](https://blog.hubspot.com/website/what-is-tailwind-css)

## Bookmark and Review
- [What is Django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction)
- [First Django App - Par1 1](https://docs.djangoproject.com/en/4.1/intro/tutorial01/)
- [First Django App - Part 2](https://docs.djangoproject.com/en/4.1/intro/tutorial02/)
- [Tailwind CSS Django - Flowbite](https://flowbite.com/docs/getting-started/django/)

## Other Material
- [Python Django Tutorial for Beginners](https://www.youtube.com/watch?v=rHux0gMZ3Eg&t=812s)
- [Django Project - Code a CRM App Tutorial](https://www.youtube.com/watch?v=t10QcFx7d5k&t=11s)

## Reading Questions

1. What are the key components of the Django framework, and how do they contribute to building a web application?
> Key components or its built-in batteries/tools include user authentication, content administration, site maps, RSS feeds and many more. The built-in components contribute to a faster development cycle and turnaround time. 
2. Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.
> Model is responsible for the data-related logic. View handles the presentation logic and user interface. View also handles the WRRC. Template handles the presentation of the data received from the View. [ChatGPT](https://chat.openai.com/c/27245498-384e-424b-8dcd-92259949105b)
3. What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?
> It is a low-level framework for quick development and customization. Some differences include ability to write it directly in your HTML, changes are local, and you can create your own reusable components and styles.

## Things I would like to learn more about
- Clickjacking, Cross-site scripting, Cross Site Request Forgery, SQL injection, Remote code execution
- [Django Developers Google Group](https://groups.google.com/g/django-developers)
- [Django issue tracker](https://code.djangoproject.com/query)
- [Django Fellow Podcast - Tim Graham](https://djangochat.com/episodes/django-fellow-tim-graham)
- [Django Fellow Podcast - Mariusz Felisiak](https://djangochat.com/episodes/django-fellow-mariusz-felisiak)
- Benevolent Dictators For Life
- [DjangoCons](https://2019.djangocon.us/)
- [Tailwind design system](https://blog.hubspot.com/website/design-system?hubs_content=blog.hubspot.com%2Fwebsite%2Fwhat-is-tailwind-css&hubs_content-cta=design%20system)
- [Tailwind Open-Source Components](https://tailwindcomponents.com/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs/customizing-colors)