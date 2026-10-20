Require() function method is used when our project type is commojs and used import method when project type is module.

app.use() -> used for middleware

req.params.(index/id/etc means dynamic value)-> params is used to access dynamic segments of the URL path (route parameters), whereas req.body is used for data sent within the HTTP request body (typically in POST, PUT, or PATCH requests). 

The key distinctions are:

Source of Data: req.params extracts values from the URL path itself (e.g., /users/:id), while req.body extracts key-value pairs from the parsed request payload (e.g., JSON or form data).
Visibility and Length: Params are visible in the URL and limited in length, making them suitable for identifying specific resources (like an ID). Body data is hidden from the URL, allowing for large or complex data structures and sensitive information.
HTTP Methods: req.params are commonly used with GET requests to fetch resources, while req.body is standard for POST/PUT requests to create or update resources. 
Using req.params is preferred for resource identification because it is RESTful and explicitly defines the resource hierarchy in the URL, whereas req.body is intended for the actual data being submitted to that resource. 