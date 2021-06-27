# Express

### What’s the difference between PUT and PATCH?
PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely. PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

For example, when you want to change the first name of a person in a database, you need to send the entire resource when making a PUT request.
```
{“first": "John", "last": "Stone”}
```

To make a PUT request, you need to send the two parameters; the first and the last name.

Unlike PUT, PATCH applies a partial update to the resource.

This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. So if you want to update the first name on a database, you will only be required to send the first parameter; the first name.

### Compare and contrast SOAP and ReST
* SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.
* SOAP is a protocol whereas REST is an architectural pattern.
* SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State Transfer.
* SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.
* SOAP cannot make use of REST whereas REST can make use of SOAP.
* SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.
### Provide links to 3 services or tools that allow you to “mock” an API for development like json-server.

[Postman](https://www.postman.com/)
[Swagger](https://apibldr.com/?gclid=CjwKCAjww-CGBhALEiwAQzWxOnpF3iJAR1SxT5PPs07-rVMdEWRjDxd_yLeiSMLicD6jt_Tnzk1ntxoCKOUQAvD_BwE)
[Mocky](https://designer.mocky.io/)

### Document the following Vocabulary Terms
* SOAP: is a protocol which was designed before REST and came into the picture. The main idea behind designing SOAP was to ensure that programs built on different platforms and programming languages could exchange data in an easy manner. SOAP stands for Simple Object Access Protocol.
* ReST Verbs: specify an action to be performed on a specific resource or a collection of resources.
* CRUD Verbs: major portion of our “uniform interface” constraint and provide us the action counterpart to the noun-based resource.
* Swagger: Swagger is in essence an Interface Description Language for describing RESTful APIs expressed using JSON.
### Express Routing
* This is an event driven system
Same routing patter as vanilla JS and JQuery
* When a get event happens on “/thing”, run this function…
* The request object will accept Parameters and Query Strings
* The response object is responsible for sending data back to browser
* Responses include headers, cookies, and status codes
### Express Middleware
* Middleware is a series of functions that the request moves through
* Each receives request, response and next as parameters
* Two types - Application and Route
 ### Application
* Error handling
* Bringing in other routes
* Applies Defaults
* JSON, Body and Form parsing
* Runs on every request
### Route
* Specifically for a route
* Are you logged in?
* What is your IP?
* Have we seen you here before?
### Modularization & Separation of Concerns
* Modularize code into logical chunks
* Each thing should do the thing it is best at
### CRUD Operations with REST and Express
* CREATE - app.post(‘/resource’)
* READ - app.get(‘/resource’)
* UPDATE - app.put(‘/resource/:id’)
* DELETE - app.get(‘/resource/:id’)
### Server Testing
* Avoid starting actual server for testing
* Export server as a module in a library
* Use supertest to run tests
* Hits routes as though server is running without starting it
* One less thing to go wrong (eliminate variables)
* Wrap superagent in a module that persons this
* 100% fake every call to the API
* Only tests the interface to the API, not actual data
### Test Pyramid
* Server Testing
  * Units - Server Internal Functions
  * Mock integrations
* Integration - How it connects to other services
  * Hard dependencies
* Acceptance
  * Server might be a dependency of another test
### What is Middleware?
* Functions invoked by the Express.js routing layer before final request handler is made
* On a route, do something first, then pass it along to the next function
* Request and Response used each time to pass to the next whatever it is being handled
* Deal with CORS or CSRF issues first, check to see if user is authorized, and then send them where they want to go
* App.use runs middleware on all requests
* Can declare middleware functions wherever in file due to hoisting