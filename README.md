# Flask-documentation
## what is flask:.
Flask is a web framework, it’s a Python module that lets you develop web applications easily. 
It’s has a small and easy-to-extend core, it’s a microframework 
Flask is a web application framework written in Python
Unlike the Django framework, Flask is very Pythonic. It’s easy to get started with Flask,
because it doesn’t have a huge learning curve.


## Requirement---------------------------------------
#### 1-) Python Version:

We recommend using the latest version of Python. Flask supports Python 3.6 and newer.

#### 2-) other Dependencies distributions will be installed automatically when installing Flask:

- Werkzeug 
- Jinja 
- MarkupSafe 
- ItsDangerous
- Click
	
## Installation---------------------------------------------

## 1-) install python:
	
[get the latest version](https://www.python.org/ftp/python/3.10.0/python-3.10.0-amd64.exe)
	
## 2-) use virtual enviroment:

to start our project its recommended to use virtual enviroment to manage the dependencies for your project, both development and in production.
Virtual environments are independent groups of Python libraries, one for each project.
Packages installed for one project will not affect other projects or the operating system’s packages.
Python comes bundled with the venv module to create virtual environments.
	
### Create an environment:

Create a project folder and a venv folder within:
	
#### in windows----------

		 mkdir myproject
		 cd myproject
		 py -3 -m venv venv
		
#### in linux-------------

		 mkdir myproject
		 cd myproject
		 python3 -m venv venv
		
### Activate the environment:

#### in windows----------

		 venv\Scripts\activate
		
#### in linux-------------

		 source venv/bin/activate
		
Your shell prompt will change to show the name of the activated environment(venv).

## 3-) Install Flask:

	 pip install Flask
	
  Flask is now installed, in the python and we can use it by export it in the python comand like:
  
	 python import Flask
	 exit()
	
## 4-) creat a file in our folder and name it as falsk-proj.py

First we imported the Flask class. An instance of this class will be our WSGI application.

	from flask import Flask, render_tamplate

Next we create an instance of this class. The first argument is the name of the application’s module or package.
__name__ is a convenient shortcut for this that is appropriate for most cases.
This is needed so that Flask knows where to look for resources such as templates and static files.

	app = Flask(__name__)
	
We then use the route() decorator to tell Flask what URL should trigger our function.
and function called index with to render the index.html flie.

	@app.route("/index.html")
	
	def index():
            return render_tamplate("index.html")
	
open the folder with vs-code, then create a template folder, add new file and name it as "index.html" and wirte inside of it our code.

wirte a test code in the file such like:
	
	<h1> htis is the test code </h1>

5-) start up the server:

in windows----------

	 set FLASK_APP=falsk-proj
	 set FLASK_DEBUG=1
	 flask run

in linux-------------

	 export FLASK_APP=falsk-proj
	 export FLASK_DEBUG=1
	 flask run


