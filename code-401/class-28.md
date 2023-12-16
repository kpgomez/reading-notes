# Class 28 - Readings: Django CRUD and Forms

## Sources
- [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)
- [Legacy Notes]()

## Bookmark and Review
- [Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)
- [Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)

## Reading Questions
- [ChatGPT Summary](https://chat.openai.com/c/f4c173c2-2340-4c5a-922a-215fc665cb7b)
1. How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?
> Django Forms simplifies the previous process of working with forms. Developers no longer need write the HTML for the form, write validation rules, implement error handling, etc. Django Forms abstracts all of that and enable the developers to quickly define forms and their fields programmatically. Key components include Django's Form class, declaration of form field types, and other arguments. 
2. Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability.
> According to ChatGPT, Django Templates are used for generating HTML dynamically. The presentation and business logic are separated. By separating the template into ancestor and child templates, you can make changes in a single location, the ancester template, that will apply across any of its child templates. This reduces having to make changes in multiple places and prevents bugs. 
3. Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views.
> Django Views handle the HTTP request and response. They also contain the logic for the processing data. The differences between the two include level of difficulty with function based being easier to implement. Class based views implement a mixin which function does not. The organization of the code is inherently differently with class based views. 