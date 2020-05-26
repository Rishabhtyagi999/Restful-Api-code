# Restful-Api-code
API Development in Python is a very easy task. This tutorial will help you to create a basic REST API in Python with the Flask Framework.

REST APIs are pretty much everywhere. They are the standard method to expose databases to clients and knowing how to develop a REST API is a necessity at all layers of the stack.

There are many reasons why you should learn to develop REST APIs in Python. If you are new to API development, then learning how to develop a REST API, will help you to showcase yourself to the industry.


REST (REpresentational State Transfer) is an architectural style, and an approach to communications that is often used in the development of Web services. The use of REST is often preferred over the more heavyweight SOAP (Simple Object Access Protocol) style because REST does not leverage as much bandwidth, which makes it a better fit for use over the Internet. The SOAP approach requires writing or using a provided server program (to serve data) and a client program (to request data).

stuffs we require to build our first REST API
Python
Flask
Flask-SQLAlchemy
Flask-Restful
SQlite3
Jsonify

Let the Code Begin
Download the dataset from the Employees and Tracks Details and extract in your project folder named 'python_rest'. Database name is "chinook.db"

Once downloaded, make a file named server.py in the python_rest folder. This file will contain the API Definitions and Flask Code.
Screen Shot 2017-02-13 at 11.17.52.png

Now, we create a basic virtual environment for Python2.7 and install the packages after it's activation.

$ virtualenv venv
$ source venv/bin/activate
$ pip install flask flask-jsonpify flask-sqlalchemy flask-restful
$ pip freeze

Screen Shot 2017-02-13 at 11.23.35.png

Let's create the basic GET API

REST has got 4 options
GET
PUT
POST
DELETE
We will deal with GET and you will get how other works .
Now everything being set up, we begin the code of exposing employees data and tracks data from database and also add a query operator on employees where employee's details is searched and fetched by EmployeeID.

