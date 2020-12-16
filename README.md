# Blog-api
Blog API using the full set of **Django REST Framework** features allows for full CRUD (Create-Read-Update-Delete) functionality. 

## Blog api endpoints 
We list all available blog posts as a read-write endpoint which means using `ListCreateAPIView`, which is similar to the `ListAPIView` but allows for writes. We also make the individual blog posts available to be read, updated, or deleted. Another built-in generic **Django REST Framework** view is used for this purpose: `RetrieveUpdateDestroyAPIView`.

* Post List endpoint: both GET and POST methods are allowed.  
http://127.0.0.1:8000/api/v1/

* Single Post endpoint: GET, PUT, and DELETE are supported.  
http://127.0.0.1:8000/api/v1/1/

##  Permissions

* Project-Level Permissions: only authenticated, or logged in, users can view the API.
* View-Level Custom Permissions: in the file, posts/permissions.py, read-only permissions are allowed for any request, but write permissions are only allowed to the author of a post.

## Token Authentication
To implement token authentication, third-party packages are used. We use **dj-rest-auth** in combination with **django-allauth** to simplify things.

Here are some endpoints.

* Log in endpoint  
http://127.0.0.1:8000/api/v1/dj-rest-auth/login/

* Log out endpoint  
http://127.0.0.1:8000/api/v1/dj-rest-auth/logout/

* User registration endpoint: here we output the emails to the console with the console.EmailBackend setting.  
http://127.0.0.1:8000/api/v1/dj-rest-auth/registration/  

![alt TT](https://github.com/pcchu30/static/blob/master/images/django_api/Register.png?raw=true)

