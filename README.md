from django.db import models


class Vikrant(models.Model):
	title = models.CharField(max_length = 200)
	description = models.TextField()

from django.db import models

class Vikrant(models.Model):
		
	title = models.CharField(max_length=200)
	description = models.TextField()
	last_modified = models.DateTimeField(auto_now_add=True)
	img = models.ImageField(upload_to=& quot
							images/"
							)

	
	def __str__(self):
		return self.title
from django.contrib import admin 

from .models import Vikrant 

admin.site.register(Vikrant)

