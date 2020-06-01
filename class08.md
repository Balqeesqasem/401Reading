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