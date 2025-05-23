# Ex02 Django ORM Web Application
## Date: 10/04/2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).
## DESIGN STEPS
## ER DIAGRAM:
![MOVIE](https://github.com/user-attachments/assets/4f7d119f-cc82-49ec-a9ad-7f2193c54ca9)



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
class Employee(models.Model):
    User_name=models.CharField(max_length=100)
    email=models.EmailField()
    Phone_Number=models.IntegerField()
    MovieName=models.CharField(max_length=100)
    seats=models.IntegerField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('User_name','email','Phone_Number','MovieName','seats')

admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)


```


## OUTPUT

![alt text](<Screenshot 2025-04-10 230834.png>)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
