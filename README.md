# Ex01 Django ORM Web Application
## Date:20/11/2025
register number: 25006451

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
~~~
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
~~~

~~~
from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)
~~~

## OUTPUT

<img width="1919" height="1079" alt="Screenshot 2025-11-20 114910" src="https://github.com/user-attachments/assets/233aec96-4cfe-459e-9533-070f4a650edf" />
<img width="1059" height="899" alt="Screenshot 2025-11-21 153010" src="https://github.com/user-attachments/assets/3320bf44-d5c0-486d-920f-e8dd299877fb" />



## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
