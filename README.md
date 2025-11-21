# Ex01 Django ORM Web Application
## Date: 21:11:2025
## 25007032

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM

models.py:

from django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]


admin.py:

from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)


## OUTPUT

<img width="1919" height="1029" alt="Screenshot 2025-11-20 150601" src="https://github.com/user-attachments/assets/6f7c9740-99c3-4100-be8c-f2ce20f32827" />

<img width="1158" height="829" alt="Screenshot 2025-11-21 152950" src="https://github.com/user-attachments/assets/081d0c23-9bbf-49c8-87b0-6eb62d898dd4" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
