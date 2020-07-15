---
title: Django Cheat Sheet
description: Made for perfectionists with deadlines.
slug: django
authors:
- comficker
updated: 2020-07-08 19:57:34 UTC
stars: 544
sheets:
- fields:
     - field: Start a project
       value: django-admin startproject project_name
- title: Start the server
  fields:
     - field: cd into your project's root directory* to start Django server the root is where your manage.py lives
       value: python manage.py runserver
- title: create an app
  fields:
     - field: An app is a directory containing code functionality able to live by itself apart from the other parts of the website
       value: python manage.py startapp app_name
- title: set urlconf
  fields:
     - field: Create a file called urls.py in your app directory and set urlpatterns
       value: urlpatterns = \[ url(r'^$', views.index, name='index'), ]
     - field: Add urls.py in your app's directory and register to let it route its internal link
       value: url(r'^app_name/', include('app_name.urls'))
---
