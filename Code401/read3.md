# Express Routing & Connected API
### Review, Research, and Discussion

1. ### Name 3 real world use cases where you’d want to change the request with custom middleware

* Authorization and validation
* fetch data from different API’s.
* Validate a data before store it in database.

2. ### True or false: The route handler is middleware? 
  ***false***

3. ### In what ways can a middleware function end the process and send data to the browser? 
 ***Sending a response that holding a data.***

4. ### At what point in the request lifecycle can you “inject” middleware? 
***Using the next() parameter that sends the data.***

5. ### What can cause express to error with “Request headers sent twice, cannot start a second response”
 ***If we send two response for the same request that would cause an error.***

### Document the following Vocabulary Terms
* Middleware : functions are functions that have access to the request object ( req ), the response object ( res ), and the next function in the application’s request-response cycle.

* Request Object: represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
* Response Object: The res object represents the HTTP response that an Express app sends when it gets an HTTP request
* Application Middleware: represented by app.use() and app.METHOD(), where METHOD is the HTTP method(in lowercase).
* Routing Middleware: works in the same way as application-level middleware, except it is bound to an instance of express.Router().

### Modularizing Routes In Express API Apps
Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.
#### Types of routes:

* Basic Routes: Home, About
* Route Middleware: to log requests to the console
* Route with Parameters
* Route Middleware for Parameters to validate specific parameters
* Login routes Doing a GET and POST on /login
* Validates a parameter passed to a certain route

### Usually we use these files as these roles:

* ``index.js -``  Entry Point.

* ``server.js -``  Hub, Exported Server.

* ``models/categories.js``,  etc - Data Models.

* ``routes/categories.js``,  etc - Routers and Handlers.

* With the inclusion of the Express 4.0 Router, we are given more flexibility than ever before in defining our routes; we can:
* Use express.Router() multiple times to define groups of routes.
* Apply the express.Router() to a section of our site using app.use().
* Use route middleware to process requests.
* Use route middleware to validate parameters using .param().
* Use app.route() as a shortcut to the Router to define multiple requests on a route.