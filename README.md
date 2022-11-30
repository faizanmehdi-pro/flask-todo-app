## TODO APP:

This is a simple TODO APP which contains the API's that performs CRUD operations on a Postgres database using Flask, Flask-RESTful, SQLAlchemy as ORM.

### Content:

todo.py - Defines the flask app, and the Flask RESTful api endpoints defined on top of it
models.py - Defines the data model, implemented with the Flask SQLAlchemy ORM

Using the api:
To access the api from the command line:

GET Request (for task with id 1):

```curl --location --request GET 'http://127.0.0.1:5000/todo/18' --header 'Authorization: Basic YWRtaW46bXlwYXNzd29yZA=='```


POST Request:

```curl --location --request POST 'http://127.0.0.1:5000/todo/' --header 'Authorization: Basic YWRtaW46bXlwYXNzd29yZA==' --header 'Content-Type: application/json' --data-raw '{"name": "Submit Assignment", "description": "The TODO APP"}'```

PUT Request:

```curl --location --request PUT 'http://127.0.0.1:5000/todo/18' --header 'Authorization: Basic YWRtaW46bXlwYXNzd29yZA==' --header 'Content-Type: application/json' --data-raw '{"name": "Submit Assignment", "description": "The TODO APP"}'```

DELETE Request:

```curl --location --request DELETE 'http://127.0.0.1:5000/todo/18' --header 'Authorization: Basic YWRtaW46bXlwYXNzd29yZA=='```

