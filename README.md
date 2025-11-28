# Ex02 Django ORM Web Application
## Date: 26.11.2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
```
models.py

from django.db import models
from django.contrib import admin
class Car(models.Model):
    regno=models.CharField(max_length=20)
    name=models.CharField(max_length=20)
    prize=models.IntegerField()
    year=models.IntegerField()
class CarAdmin(admin.ModelAdmin):
    list_display=('regno', 'name', 'prize', 'year')

admin.py

from django.contrib import admin
from . models import Car,CarAdmin
admin.site.register(Car,CarAdmin)


```

## OUTPUT

<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/edd2c119-d379-4dd8-bc33-91462d299e3a" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
