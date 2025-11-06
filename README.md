# Ex02 Django ORM Web Application
## Date: 22-09-2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="1037" height="557" alt="image" src="https://github.com/user-attachments/assets/8f195aaa-05e0-4759-aeb1-4b2f27b68113" />

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
admin.py
```
from django.contrib import admin
from .models import Car
# Register your models here.

admin.site.register(Car)

class CarAdmin(admin.ModelAdmin):
    list_display = ['id','brand','model','year','price']
```
models.py
```
from django.db import models

# Create your models here.
class Car(models.Model):
    id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models.CharField(max_length=30)
    year = models.DateField()
    price = models.IntegerField()
```


## OUTPUT

<img width="1035" height="608" alt="image" src="https://github.com/user-attachments/assets/aa72c714-8f22-4b8e-ae86-02f46637637f" />


## RESULT
Thus the program for creating a database using ORM hass been executed successfully.
