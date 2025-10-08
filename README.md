# Project Responsive Web Design using Bootstrap
# Date:
8/10/2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
html:

{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap Example</title>
  <style>
    a{
        margin-left:10px;
        text-decoration: none;
    }
    #nee{
        margin-top:6px;
        margin-left:17px;
        border-radius:10px;
    }
    #heeder{
        padding:10px;
    }
    #b1,#b2{
        border-radius:20px;
        border:2px;
        padding-left:10px;
        padding-right:10px;
    }
    .card{
        margin:20px;
    }
    #bb1,#bb2,#bb3,#bb4{
        display:inline-block;
        border-radius:30px;
        margin:0px;
        padding:0px;

    }
    img :hover{
        transform:scale(1.5);
    }
  </style>
  <!-- Bootstrap CSS -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
    rel="stylesheet">

  <!-- Bootstrap JS (for components like modals, dropdowns, etc.) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body style="background-color: rgb(202, 197, 191);">
    <nav class="navbar navbar-expand-lg navbar-light bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand text-light" href="#">Dribbble</a>
            <ul class="navbar-nav me-auto">
                <li class="nav-item"><a href="#" class="text-info nav-link active">Shots</a></li>
                <li class="nav-item"><a href="#" class="text-info nav-link">Designs</a></li>
                <li class="nav-item"><a href="#" class="text-info nav-link">Teams</a></li>
                <li class="nav-item"><a href="#" class="text-info nav-link">Community</a></li>
                <li class="nav-item"><a href="#" class="text-info nav-link">Jobs</a></li>
            </ul>
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a href="#" class="text-primary nav-link text-center">Sign in</a></li>
                <li class="nav-item"><a href="#" class="text-danger nav-link text-center">Sign up</a></li>
                <li class="nav-item"><input type="text" class="navbar-light text-center" id="nee" placeholder="Search"></li>
            </ul>
        </div>
    </nav>
    <header class="bg-secondary text-center " id="heeder">
        <ul>
        <h5 class="text-dark display-25">What are you working on? <span class="text-light">dribble is show and tell for designers</span></h5>
        <button type="submit" class="bg-primary py-1.3 px-1.3" id="b1">learn more</button>
        <button type="submit" class="bg-danger text-light py-0.9" id="b2">Sign up</button> 
        </ul>      
    </header>
    <section class="container">
        <div class="row">
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img1.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">WeGrow <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">PRO</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img2.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Designator <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">PRO</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img3.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Paperpillar <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">TEAM</span></a></h6>
            </div>    
        </div>
        </div>
        <div class="row">
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img4.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">OutCrowd <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">PRO</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img5.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Emote <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">TEAM</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img6.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Halo Lab <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">TEAM</span></a></h6>
            </div>    
        </div>
        </div>
        <div class="row">
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img7.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Steve Robolic <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">PRO</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img8.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Bro Code <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">TEAM</span></a></h6>
            </div>    
        </div>
        <div class="col-md-4">
            <div class="card bg-secondary">
                <img src="{% static 'img9.jpg' %}" alt="hi">
                <br>
                <h6 class="card-title text-center"><a href="#" class="text-decoration-none text-white">Coric Design <span style="background-color: rgb(240, 198, 214);border-radius:5px;color:rgb(14, 14, 14);font-size:13px;padding-left:4px;padding-right:4px;">PRO</span></a></h6>
            </div>    
        </div>
        </div>
    </section>
    <footer class="bg-dark container-fluid">
    <div class="row">    
        <ul class="col-md-4 text-center" id="bb1">
            <br>
            <li><a href="#" class="text-info text-decoration-none">Home</a></li>
            <li><a href="#" class="text-info text-decoration-none">Shots</a></li>
            <li><a href="#" class="text-info text-decoration-none">Designs</a></li>
            <br>
        </ul>
        
        
        <ul class="col-md-4 text-center" id="bb2">
            <br>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.digital.com</a></li>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.manager.com</a></li>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.template.com</a></li>
            <br>
        </ul>
        
        
        <ul class="col-md-4 text-center" id="bb3">
            <br>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.custom.com</a></li>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.aniga.com</a></li>
            <li><a href="#" class="text-info text-decoration-none">www.dribble.figna.com</a></li>
            <br>
        </ul>
    </div>
    </footer>
</body>
</html>
 
views:

from django.shortcuts import render
def web(request):
    return render(request,'webpage.html')

urls:

"""
URL configuration for pname project.

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/5.2/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import path
from app import views
urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.web),
]

```
# OUTPUT:
![alt text](<Bootstrap Example and 1 more page - Personal - Microsoft​ Edge 08-10-2025 20_18_29.png>)
![alt text](<Bootstrap Example and 1 more page - Personal - Microsoft​ Edge 08-10-2025 20_19_09.png>)
![alt text](<Bootstrap Example and 1 more page - Personal - Microsoft​ Edge 08-10-2025 20_19_17.png>)
![alt text](<Bootstrap Example and 1 more page - Personal - Microsoft​ Edge 08-10-2025 20_19_22.png>)



# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
