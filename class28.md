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

##### Login and Auth

    - (Links to an external site.)ROLE-BASED ACCESS CONTROL (RBAC)
    - Restricts network access based on a person's role within an organization and has become one of the main methods 
      for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
      (Links to an external site.)BENEFITS OF RBAC
      Reducing administrative work and IT support.
      Maximizing operational efficiency.
      Improving compliance.
      Isomorphic cookies

     - To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie.


## Basic Authorization

      - Basic Authorization is a common method used to send a username and password in an HTTP request. The username and
        password are joined with a ‘:’ then “base64 encoded” and placed after the string ‘Basic ‘. The resulting string is set to the value of an Authorization header.   
      - A Server can decode the Basic Authorization header to retrieve the username and password. If the combination is
        validated, the server generally responds back to the client with some sort of validation response (token or key) 
        so that the client can re-authenticate without having to continually send the username:password combination in 
        plain text over the internet. 

        #### base64 encoding is not a form of encryption. The client and server must use HTTPS to protect the username 
             and password as it travels across the network. 


## Login and Auth
      - ContextAuthentication + Role Based Authorization
      - we check if the valid user is loggend in and what is the user authorized to do, Which parts care about this,
        What’s in the token,Contact between the UI and the API, How do we make this easy to use , <Auth /> it about permissions and login status,give access to a component or jsx or hides it, we dont use redux don’t want to force implementors into a specific state management system.       
                    
         