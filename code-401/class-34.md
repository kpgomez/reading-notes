# Class 34: API Deployment

## Sources
- [Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)

## Bookmark and Review
- [White Noise](https://whitenoise.readthedocs.io/en/stable/)
- [CORS](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)

## Reading Questions
1. What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?
> Keep all Django setting configurations, sensitive data should not be stored in VCS, a way to share settings between team members, store configuration in the environment
- [ChatGPT](https://chat.openai.com/c/baa8f552-30fb-49bd-ae7f-40f633bd2558)
2. How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project? 
> According to ChatGPT, it compresses static files on the fly and cache headers for static files. By processing the data in advance, it acts like dictionary look-up when serving files.
3. What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?
- [ChatGPT](https://chat.openai.com/c/a26d0592-3776-40b3-a0b0-dde6230d88bf)
> According to ChatGPT, CORS allows servers to specify allowed parties and terms for accessing resources. To implement, install django-cors-headers, add corsheadeers to INSTALLED_APPS, update MIDDLEWARE, configure CORS_ALLOWED_ORIGINS.