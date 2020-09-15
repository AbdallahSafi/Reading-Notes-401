## Express Routing & Connected API

#### Modularizing Routes In Express API Apps

  - Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.
  - Types of routes: 
   * **Basic Routes**: Home, About
   * **Route Middleware**: to log requests to the console
   * **Route with Parameters**
   * **Route Middleware for Parameters** to validate specific parameters
   * **Login routes** Doing a GET and POST on /login
   * Validates a parameter passed to a certain route

  - Usually we use these files as these roles: 
    * `index.js` - Entry Point.
    * `server.js` - Hub, Exported Server.
    * `models/categories.js, etc` - Data Models.
    * `routes/categories.js, etc` - Routers and Handlers.


- With the inclusion of the Express 4.0 Router, we are given more flexibility than ever before in defining our routes; we can: 
    * Use express.Router() multiple times to define groups of routes.
    * Apply the express.Router() to a section of our site using app.use().
    * Use route middleware to process requests.
    * Use route middleware to validate parameters using .param().
    * Use app.route() as a shortcut to the Router to define multiple requests on a route.
