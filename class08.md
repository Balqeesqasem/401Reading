# Express 4.0

  - Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like .use, .get, .param, and route.

### Starting Our Application:
   - install express.
   - Creating Our Server

###  Express Router
  
  - What exactly is the Express Router? It is a mini express application without all the bells and whistles of an express application, just the routing stuff.  

###  Route Middleware router.use()
 
 - Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.

             - Use express.Router() multiple times to define groups of routes
             - Apply the express.Router() to a section of our site using app.use()
             - Use route middleware to process requests
             - Use route middleware to validate parameters using .param()
             - Use app.route() as a shortcut to the Router to define multiple requests on a route


         With all the ways we can define routes, I'm sure that our applications will benefit going forward. Sound off in the comments if you have any questions or suggestions.



    * With the inclusion of the Express 4.0 Router, we are given more flexibility than ever before in defining our  
      routes. 
      
      
      
      
  ## Routing

     - Routing is how an application’s endpoints (URIs) respond to client requests. 

     - Routing refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on).

     - Each route can have one or more handler functions, which are executed when the route is matched.

#### Route methods

     - A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

#### Route paths

     - Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

#### Route parameters

     - Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

#### Route handlers

     - You can provide multiple callback functions that behave like middleware to handle a request. The only exception is that these callbacks might invoke next('route') to bypass the remaining route callbacks. You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there’s no reason to proceed with the current route.
     
     - Route handlers can be in the form of a function, an array of functions, or combinations of both.

#### Response methods

     - The methods on the response object (res) in the following table can send a response to the client, and terminate the request-response cycle. If none of these methods are called from a route handler, the client request will be left hanging.
    
