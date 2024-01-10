# Class 33: Authentication & Production Server

## Notes
JSON Web Tokens consist of three parts; Header, payload, signature separated by a decimal point/dot. 

<u>**Header**</u> is composed of signing algorithm and type of token

Example
```json
{
    "alg": "HS256", <!-- signing algorithm -->
    "typ": "JWT" <!-- type of token -->
}
```

Signing algorithms; HMAC SHA256, RSA

<u>**Payload**</u> contains the claims

Three types of claims; registered, public, and private

Registered is predefined, not mandatory but recommended

Public is defined at will

Private is neither registered or public, but custom and created to share information

Example
```json
{
    "sub": "1234567890",
    "name": "John Doe",
    "admin": true
}
```

<u>**Signature**</u> is used to verify contents were not tampered during exchange and to authenticate sender

Example
```json
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
```

![Alt text](image-22.png)

<u>**Mitigating Security Concerns:**</u>
- Do not include sensitive information in the payload or header unless encrypted
- Do not store sensitive session data in browser storage

<u>**Benefits of JSON**</u>
- less verbose than XML
- when encrypted is more compact than SAML
- easier to parse

<u>**JWT example after** ***Bearer***</u>
```curl
curl http://127.0.0.1:8000/hello/ -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTQzODI4NDMxLCJqdGkiOiI3ZjU5OTdiNzE1MGQ0NjU3OWRjMmI0OTE2NzA5N2U3YiIsInVzZXJfaWQiOjF9.Ju70kdcaHKn1Qaz8H42zrOYk0Jx9kIckTn9Xx7vhikY'
```
Secret keys check and validate the signature

## Sources
- [Reading: JSON Web Tokens](https://jwt.io/introduction/)
- [Reading: DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)
- [Reading: Django Runserver Is Not Your Production Server White Noise](https://vsupalov.com/django-runserver-in-production/)
- [YT Video: JWT with DRF ](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)

## Bookmark and Review
- [Gunicorn](https://gunicorn.org/)
- [RealPython: Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)

## Reading Questions
1. What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?
> Their primary purpose is to authenticate the identity of sender and check for authorization of access to different resources
2. How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?
> You can integrate JWT authentication within Django REST Framework by updating the project configuration files.

> Step one, `pip install djangorestframework_simplejwt`. 

> Step two, update settings.py. 

```python
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}
```
> Step three, update urls.py

```python
from django.urls import path
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]
```

> Then update views.py and urls.py within the app directory

3. Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?
> Django's built-in server is not performant and is insecure. Production grade servers are reliable, well-tested, and in use for a good while. A good alternative is Nginx and Gunicorn.

## Things I want to learn more about
- Base64-URL
- CORS