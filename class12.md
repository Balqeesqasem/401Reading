### OAuth
 
   -  is an open standard for access delegation.
   - OAuth serves as a way to give users the ability to grant application access to services, without giving the 
     application their password.



##### How does OAuth work?
        
        Through a series of “handshakes”, an application such as an Express Web Server asks the user if it’s ok to login as them at some remote service, and then begins the process of authentication and access.

              - Application spawns the “Login Using xxx” window, asking for specific permissions
              - User Agrees to allow this to happen
              - Remote service (i.e. Google) contacts the application with a one-time-use Code
              - The application calls back to a special address on the remote service to exchange that Code for a Token.
              - Once the token has been granted, the application will then be able to contact the remote service, using that Token to access information on behalf of the user    
              
               