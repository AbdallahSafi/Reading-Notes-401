## Express Routing

* Event Driven System: when a get event happens on the server, check the route and run the function associated with that route
```
app.get('/thing', (req,res) => {})
```

* The Request Object can take Parameters (:params) and Query Strings (?key=value)

* The Response Object is responsible for sending data back to the browser
  - Can send Headers with Cookies and Status Codes

## Express Middleware

* Middleware can be divided into two categores:

  - *Application Middleware* includes error handling, bringing in other routes, applying defaults, JSON/Body/Form Parsing

  - *Route Middleware* deals with specific information for a route, such as are you logged in?  Is it your first time on this route?  What is your IP?

## CRUD Operations with REST and Express

|REST Method|CRUD Operation|Express Method Route|Function|
|:-:|:-:|:-:|:--|
|POST|CREATE|app.post('/resource')|Create a New Record|
|GET|READ|app.get('/resource')|Retrieve 1+ Records|
|PUT|UPDATE|app.put('/resource/:id')|Replace Record with an updated version|
|DESTROY|DELETE|app.get('/resource/:id')|Remove a Record|

## Server Testing

* Best practice is to export your server as a module in a library and then use 'supertest' to run tests through the server without actually having to start the server for testing.  This limits the variables involved in the test

* Similarly, 'superagent' can be wrapped in a module for testing so that the API is not actually called during server tests

## Test Pyramid

* Units: Server Internal Functions
* Integration: How it connects to other services
* Acceptance

## [Express.js Fundamentals - 6 - Middleware Explained](https://www.youtube.com/watch?v=9HOem0amlyg)

* **middleware**: Any number of functions that are invoked by the Espress.js routing layer before your final request handler is made

  - All middleware functions carry an optional 'next' parameter, which is needed when passing along the request to the next function in the chain

