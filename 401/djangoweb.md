# JSON Web:
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
![img](https://cdn2.auth0.com/docs/media/articles/api-auth/client-credentials-grant.png)

for more info: [JSON Web ](https://jwt.io/introduction/)

to setup fellow this TUTORIAL [TUTORIAL](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

# Django Runserver Is Not Your Production Server:

You’ve been running your app locally with `python manage.py runserver` That’s a fine command, built for development convenience, but it’s not meant to be used as part of a production setup.

If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like Gunicorn.

If you plan on running on Heroku, a web server is provided implicitly. You don’t have to take care of it. You just need to specify a command to run your application server (again, Gunicorn is fine) in the Procfile.

for more : [Django Runserver Is Not Your Production Server](https://build.vsupalov.com/django-runserver-in-production/)
