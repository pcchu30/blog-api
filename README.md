# Blog-api
Blog API using the full set of **Django REST Framework** features allows for full CRUD (Create-Read-Update-Delete) functionality. 

## Blog api endpoints 
We list all available blog posts as a read-write endpoint which means using `ListCreateAPIView`, which is similar to the `ListAPIView` but allows for writes. We also make the individual blog posts available to be read, updated, or deleted. Another built-in generic **Django REST Framework** view is used for this purpose: `RetrieveUpdateDestroyAPIView`.

* Post List endpoint: both GET and POST methods are allowed.  
http://127.0.0.1:8000/api/v1/ 

