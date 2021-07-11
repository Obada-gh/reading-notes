# Django Models:
A Django model is the built-in feature that Django uses to create tables, their fields, and various constraints. In short, Django Models is the SQL of Database one uses with Django. SQL (Structured Query Language) is complex and involves a lot of different queries for creating, deleting, updating or any other stuff related to database. Django models simplify the tasks and organize tables into models. Generally, each model maps to a single database table.
This article revolves about how one can use Django models to store data in the database conveniently. Moreover, we can use admin panel of Django to create, update, delete or retrieve fields of a model and various similar operations. Django models provide simplicity, consistency, version control and advanced metadata handling. Basics of a model include –

1. Each model is a Python class that subclasses django.db.models.Model.
2. Each attribute of the model represents a database field.
3. With all of this, Django gives you an automatically-generated database-access API; see Making queries.

Example:

```

from django.db import models
  
# Create your models here.
class GeeksModel(models.Model):
    title = models.CharField(max_length = 200)
    description = models.TextField()

```

![djangoModels](https://media.geeksforgeeks.org/wp-content/uploads/20191220123439/django-models.png)


Using Django Models:

To use Django Models, one needs to have a project and an app working in it. After you start an app you can create models in app/models.py. Before starting to use a model let’s check how to start a project and create an app named geeks.py

Creating a Model :

```
Syntax

from django.db import models
        
class ModelName(models.Model):
        field_name = models.Field(**options)
To create a model, in geeks/models.py Enter the code,

# import the standard Django Model
# from built-in library
from django.db import models
  
# declare a new model with a name "GeeksModel"
class GeeksModel(models.Model):
        # fields of the model
    title = models.CharField(max_length = 200)
    description = models.TextField()
    last_modified = models.DateTimeField(auto_now_add = True)
    img = models.ImageField(upload_to = "images/")
  
        # renames the instances of the model
        # with their title name
    def __str__(self):
        return self.title

```

# Django admin site:

The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data. The admin application can also be useful for managing data in production, depending on the type of website. The Django project recommends it only for internal data management (i.e. just for use by admins, or people internal to your organization), as the model-centric approach is not necessarily the best possible interface for all users, and exposes a lot of unnecessary detail about the models. 


```
from django.contrib import admin

# Register your models here.

from .models import Author, Genre, Book, BookInstance

admin.site.register(Book)
admin.site.register(Author)
admin.site.register(Genre)
admin.site.register(BookInstance)

```


