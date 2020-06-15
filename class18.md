# Web Sockets

   - communication Protocol which provides bidirectional communication between the Client and the Server over a TCP connection
   - WebSocket remains open all the time so they allow the real-time data transfer. 
   - When clients trigger the request to the Server it does not close the connection on receiving the response, it 
     rather persists and waits for Client or server to terminate the request.

# Socket.io 

   -  library which enables real-time and full duplex communication between the Client and the Web servers.
   -  uses the WebSocket protocol to provide the interface.
   -  WebSocket divided into two parts:
            1. Client Side: it is the library that runs inside the browser.
            2. Server Side: It is the library for Node.js.

# Connections

   - In Socket.io, you connect to a server over HTTP. The session is “kept alive” through it’s internal use of the 
     WebSocket Protocol, with session information being preserved.

   - Standard node events are sent with emit() and received with on() … Socket.io uses the same methodology/terminology.

   