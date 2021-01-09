## Getting started with Python's Flask framework.

If you want to develop web apps with python, there is a probability you will be using Frameworks. A Framework is a collection of code libraries that makes software development easier by providing reusable code. Using a framework to develop application allows you to focus on high-level functionality because most low-functionality has been taken care of by the framework.
There are a number of frameworks for web development in Python, including  [Flask](https://flask.palletsprojects.com/en/1.1.x/),  [Tornado](https://www.tornadoweb.org/en/stable/),  [Fast Api](https://fastapi.tiangolo.com/), [Pyramid](https://trypyramid.com/), and [Django](https://www.djangoproject.com/).

In this article, I will show you how to get started with flask, explain the basics and point out some useful resources. 

Flask is a small and powerful web framework for Python. It's easy to learn and simple to use, enabling you to build your web app in a short amount of time.

### Flask startup and configuration

Flask package is installable from the Preferred Installer Program (PIP). First, create a directory to work in (mysite) then install the flask package. 
I will advise you to create a Python 3 virtual environment - an isolated environment for Python projects. This means that each project can have its own dependencies, regardless of what dependencies every other project has.



%[https://gist.github.com/temitayopelumi/b4011c603838bc1921e597022a15a77d]

After installing flask,  we need to set up the Project Structure.

Create a file called  app.py inside the mysite folder this will contain our routes -  create a new folder inside the mysite folder it will contain the view of the site. 

#### The App Object

It is an instance of the Flask object. It'll act as the central configuration object for the entire application. It's used to set up pieces of the application required for extended functionality, e.g., a database connection and help with authentication.
It's regularly used to set up the routes that will become the application's points of interaction.

#### Routes and View Functions in Flask Framework Instance

Clients send requests to the webserver, which in turn, sends them to the Flask application instance.

The instance needs to know what code needs to run for each URL requested, keeps a mapping of URLs to Python functions.

The association between a URL and the function that handles it is called a route, most convenient way to define a route in a Flask application is through the (app.route).

Let's create an app instance and a basic route in our app.py


%[https://gist.github.com/temitayopelumi/f9a82eb04552840aa55c5c1381db9197]

#### Server Startup 

The application instance has a ‘run’ method that launches flask’s integrated development webserver.

Completing the app.py file.


%[https://gist.github.com/temitayopelumi/75fed6a7adfccb1b23ee4c653ff79002]
This is a complete Flask app. Once you run the scripts, it waits for requests and services in a loop.
Flask starts the server listening on 127.0.0.1 and port 5000 by default.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1610198099514/yTNN1ebIS.png)

Congratulations, you have created a simple website with the flask framework.

### Resources

1. [Flask official documentation](https://flask.palletsprojects.com/en/1.1.x/):   This is the best resource to learn about flask because it contains everything you need. Whether you are a beginner or an expert you will find yourself in their guidance.

2. [Miguel course]( https://courses.miguelgrinberg.com/p/flask-mega-tutorial): This is a paid course on the flask. The course is great especially for beginners, you learn by building some real-world web applications, from Blog to web APIs, after covering it, you can find yourself at the level of intermediate in flask framework.

3. [simplectc projects](https://simplectic.com/projects/flask-todomvc/): this is a series starting with the Backbone.js TodoMVC example and building a backend with Flask.

4. [Discover Flask](http://discoverflask.com):  An hands-on flask tutorial that takes from beginner to experts.

5. [Real python](https://realpython.com/learning-paths/flask-by-example/): Real Python takes an experiential, learning by doing approach so you build interesting projects.

6. [Build a saas app with flask](https://buildasaasappwithflask.com/): Learn to build Web applications with Flask and Docker. You will build a real-world app that accepts payments and so much more.

In this article, I barely scratch the surface web development of flask. But the goal was never to be comprehensive. Rather, I am interested in pointing other enthusiasts to great resources in order to learn more.






