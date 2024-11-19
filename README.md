# Ex02 Django ORM Web Application
## Date: 19-11-2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![WhatsApp Image 2024-11-19 at 15 39 20](https://github.com/user-attachments/assets/8bba76ff-fa0f-4b91-8c52-304a4d0a49be)


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

## admin.py

```
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)

```
## models.py
```
from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    accno=models.IntegerField(primary_key=True);
    name=models.CharField(max_length=100);
    loanamt=models.IntegerField();
    loanlimit=models.IntegerField();
    phoneno=models.IntegerField();

class bankloanAdmin(admin.ModelAdmin):
    list_display=('accno','name','loanamt','loanlimit','phoneno')

```


## OUTPUT


![Screenshot 2024-11-19 153618](https://github.com/user-attachments/assets/00fcd389-eb7a-4ca5-9ae7-b748964d2fd7)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
