# Django Custum User Model:

for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

[doc](https://docs.djangoproject.com/en/3.1/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project)

```
Setup
To start, create a new Django project from the command line. We need to do several things:

create and navigate into a dedicated directory called accounts for our code
install Django
make a new Django project called config
make a new app accounts
start the local web server
Here are the commands to run:

$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver

```
[tutorial](https://learndjango.com/tutorials/django-custom-user-model)


# DjangoX:

from [William Vincent](https://wsvincent.com/djangox-new-starter-framework/):
I recently open-sourced DjangoX which is my own opinionated starter framework for new Django projects. It comes with a custom user model by default, email/password authentication instead of Django’s default and outdated username/email/password pattern, and is fully extendable with social authentication like Gmail, Facebook, and more.