# Ex02 Django ORM Web Application
## Date: 

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
from django.db import models
from django.contrib import admin

class Car_DB(models.Model):
    car_brand=models.CharField(max_length=10)
    order_id=models.IntegerField(primary_key=True)
    car_model=models.CharField()
    price=models.IntegerField()

class Car_DBAdmin(admin.ModelAdmin):
    list_display=["car_brand","order_id","car_model","price"]


## OUTPUT

<img width="1920" height="1080" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/66a24e30-c5ec-493b-92cf-bc6951b8889c" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
