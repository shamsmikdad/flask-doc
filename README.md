# flask-doc
what is flask :
Flask is a web framework, it’s a Python module that lets you develop web applications easily. 
It’s has a small and easy-to-extend core, it’s a microframework 
Flask is a web application framework written in Python
Flask is often referred to as a microframework. It is designed to keep the core of the application simple and scalable.

Instead of an abstraction layer for database support, 
Flask supports extensions to add such capabilities to the application.
Unlike the Django framework, Flask is very Pythonic. It’s easy to get started with Flask,
because it doesn’t have a huge learning curve.

On top of that it’s very explicit, which increases readability.

Requirement---------------------------------------
1-) Python Version
    We recommend using the latest version of Python. Flask supports Python 3.6 and newer.
2-) other Dependencies distributions will be installed automatically when installing Flask:

-Werkzeug implements WSGI, the standard Python interface between applications and servers.

-Jinja is a template language that renders the pages your application serves.

-MarkupSafe comes with Jinja. It escapes untrusted input when rendering templates to avoid injection attacks.

-ItsDangerous securely signs data to ensure its integrity. 
This is used to protect Flask’s session cookie.

-Click is a framework for writing command line applications. 
It provides the flask command and allows adding custom management commands.

Installation---------------------------------------------
1-) install python latest version (https://www.python.org/ftp/python/3.10.0/python-3.10.0-amd64.exe)
2-) to start our project its recommended to use virtual enviroment to manage the dependencies for your project, both development and in production.
	Virtual environments are independent groups of Python libraries, one for each project. Packages installed for one project will not affect other projects or the operating system’s packages.
	Python comes bundled with the venv module to create virtual environments. 
	(Create an environment)
	Create a project folder and a venv folder within:
	in windows----------
		> mkdir myproject
		> cd myproject
		> py -3 -m venv venv
	in linux-------------
		$ mkdir myproject
		$ cd myproject
		$ python3 -m venv venv
	Activate the environment:
	in windows----------
		> venv\Scripts\activate
	in linux-------------
		$ . venv/bin/activate
	Your shell prompt will change to show the name of the activated environment(venv).
3-)Install Flask:
	$ pip install Flask
   Flask is now installed, in the python and we can use it by export it in the python comand like:
	python import Flask,
4-) creat afile in our folder and name it as falsk-proj.py

