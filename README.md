# Ex02 Django ORM Web Application
## Date: 18/11/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WEB PHOTO 1](https://github.com/user-attachments/assets/2d32d79d-51a0-48db-bd5d-3970aa9084d6)

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
class Costumer(models.Model):
  cid=models.CharField(max_length=20,primary_key="eid")
  accountnumber=models.IntegerField()
  name=models.CharField(max_length=20)
  age=models.IntegerField()
  address=models.CharField(max_length=50)
  phonenumber=models.IntegerField()


class CostumerAdmin(admin.ModelAdmin):
  list_display=('cid','accountnumber','name','age','address','phonenumber')

from django.contrib import admin 
from.models import Costumer,CostumerAdmin
admin.site.register(Costumer,CostumerAdmin)

## OUTPUT
![WhatsApp Image 2024-11-18 at 1 31 42 AM](https://github.com/user-attachments/assets/18669e24-be47-4818-ab0c-3ebf06965fb5)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
