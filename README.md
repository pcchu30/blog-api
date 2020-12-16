# blog-api
Blog API using the full set of `Django REST Framework` features allows for full CRUD (Create-Read-Update-Delete) functionality. 
For my Blog API, I list all available blog posts as a read-write endpoint which means
using ListCreateAPIView, which is similar to the ListAPIView but allows for writes. I also make the individual blog posts available to be read, updated, or deleted. Another built-in generic Django REST Framework view is used for this purpose: RetrieveUpdateDestroyAPIView.
