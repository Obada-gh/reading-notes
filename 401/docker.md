# Docker:
Docker which is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.

* Docker is a way to run Linux containers
* Containers are a lightweight alternative to Virtual Machines
* Dockerfile is a list of instructions for creating an image
* Images are made up of one or more layers
* Containers are a running instance of an image
* docker-compose.yml controls how to run the container
* Containers are stateless and ephemeral in nature. We can link the  local filesystem via volumes but things become more complex with databases (which we didn’t cover here).

![image](https://thingsolver.com/wp-content/uploads/pasted-image-0-768x452-1.png)

[guid to docker](https://wsvincent.com/beginners-guide-to-docker/)

# Chapter 2: Library Website and API:

Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

[toutorial](https://djangoforapis.com/library-website-and-api/)
