# AmitSoni_Python_Flask_Student_Exam_Management_Project
Python Flask Student Exam Management Project . URL: http://127.0.0.1:5000/ For Home Page .
There are Two Button on Home Page One For Create Student and Another for Showing the list of the Students .  
This Project Uses Methods POST and GET.
This Project is based on CRUD (CREATE, READ, UPDATE, DELETE) Data .
Pagination, Search Bar and Sorting by Name is also Done in this project .
Python Flask Framework, HTML, CSS, and sqlAlchemy used in this project .  
......
Home Page on : 127.0.0.1:5000

 ![home](https://user-images.githubusercontent.com/120723916/211254494-01fc692e-6427-49cd-ae21-a15f9f56db9a.png)

By clicking on create student button You will be redirected to Registration Page, URL : 127.0.0.1:5000/create 

![registration](https://user-images.githubusercontent.com/120723916/211254666-e1d9d16a-cb15-4a71-a2d3-4082fbc55753.png)

When Student Added by the user it will automatically redirect you to the students list page where you have the option for updating and deleting the Data, URL : 127.0.0.1:5000/students

![list1](https://user-images.githubusercontent.com/120723916/211254909-e7c714c2-51d0-4fa4-a064-59fe104f54dc.png)

Pagination is also Done

![pagination](https://user-images.githubusercontent.com/120723916/211255144-28f5d4c1-3cb8-4ceb-b26b-9925d2983de7.png)

Sorting Button is also given to sort the Data by the name

![sort](https://user-images.githubusercontent.com/120723916/211255205-493231ab-dff9-4e91-a91c-67d6c27c3912.png)
<hr>
<h2> Usage </h2>

```
  from flask import Flask,render_template,request,redirect,url_for,flash
  from flask_sqlalchemy import SQLAlchemy
  @app.route("/")
  #returns homepage
  @app.route("/create")
  #return student registration page
  @app.route('/students',methods=['GET','POST'])
  #returns student list page
  @app.route('/insert',methods = ['POST'])
  #for adding the students data in registration form
  @app.route('/update',methods = ['GET','POST'])
  #for updating the data
  @app.route('/delete/<id>/', methods =['GET','POST'])
  #for deleting the data
  @app.route("/sort")
  #returns sorted list
```
<h2> Deployment </h2>

If you want to deploy this application in our local system we need to follow this below steps<br>
1. We need to download python and any IDE and the modules in it as per required.<br>
2. Then need to pull the code and execute it in the system.



