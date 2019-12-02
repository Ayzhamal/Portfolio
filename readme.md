
Author: 	Angie Ayzhamal Zhamangaraeva
Date:   	December 1, 2019 
Course: 	CS 4300 Web Programming
Assignment: Project 3 "Build your own website"
Professor:  Yuchou Chang, University of Houston-Downtown 


Description: 	This website represents my portfolio page on the web. It aims to showcase the projects (mobile app, REU, research at university) I completed in the past and my hobbies (languages, traveling, hiking). On the main page, one can click to email me, or link to access my LinkedIn page, my profile picture, and the list of my projects and hobbies. 

Admin: 			Admin page available at http://www.ayzhamal.com/admin/. Admin can enter/update/delete "users" and "jobs". Job is a project or hobby which will be stored in SQLite database and output on the main page. Each job consists of a picture and a short description.


Deployment:		 The website is deployed at www.ayzhamal.com using Heroku (cloud platform as a service PaaS) and AWS S3 storage bucket to keep static files (pictures for each job). 

GitHub:			 Source code is pushed to https://github.com/Ayzhamal/Portfolio 

Tools: 			 My portfolio-website was developed on a Korean cloud goorm (https://ide.goorm.io, it allows up to 5 containers with 10GB for free) with Python Django web-framework.

Techniques: 	MVC (MTV) design pattern. M- model is models.py to build an interface between class objects and database entities, T- template in HTML files, V- views.py to render filtered data from databases
				HTMLL5 (links, images, list etc)
				CSS (bootstrap, fonts, size, color etc)
				JavaScript (selection, function, array, objects etc)
				DOM

File Structure:	Portfolio_project folder contains the following files and folders:
				"manage.py" file which allows to run administrative tasks like "python manage.py runserver", "django-admin startproject" etc. 
				"requirements.txt" includes all dependencies needed to run the website 
				"Portfolio" with settings.py with configuration details, urls.py with routing mechanisms
				"jobs" is an application folder with models.py with model classes representing an object saved in the SQLlite database, views.py is responsible for rendering needed information for each HTTP request. It uses Python Django built-in class-based views. 
				"static" is a folder with CSS, js files and my picture that pops up in the jumbotron.
				"templates" is a folder with HTML templates that use the information rendered by views from the database.  







