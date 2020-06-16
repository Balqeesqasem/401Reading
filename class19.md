#  Message Queues

     - A Queue server runs independently, and is tasked with routing events and messaging between clients.
     - Any connected client can “publish” a message into the server.
     - Any connected client can “subscribe” to receive messages by type.
     - The Queue server has the ability to see which clients are connected, to which Queues they are attached and 
       further, to which events they are subscribed.

     - The Queue server is tasked with receiving any published message and then distributing it out to all connected and subscribed clients. It must further ensure that subscribed clients can “catch up” and pull down any messages that they might have missed during a period of disconnection with the server

#  What is a message?

     - A message is a package of information, categorized by queue and event queue 
     - An API server responds to a POST request User’s access rights are confirmed The data is analyzed and normalized
       The data is sent to the database for saving The database “publishes” a message into the queue.
