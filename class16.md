# Event-Driven Programming

   - logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.Node.js uses events heavily and it is also one of the reasons why Node.js is pretty fast compared to other similar technologies. As soon as Node starts its server, it simply initiates its variables, declares functions and then simply waits for the event to occur.
   In an event-driven application, there is generally a main loop that listens for events, and then triggers a callback function when one of those events is detected.

#### EventEmitter

  - Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming 
    in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

### How Node Applications Work?
  - In Node Application, any async function accepts a callback as the last parameter and a callback function accepts an error as the first parameter. Let's revisit the previous example again. Create a text file named input.txt with the following content.


  - addListener(event, listener)

      - Adds a listener at the end of the listeners array for the specified event. No checks are made to see if the listener has already been 
        added. Multiple calls passing the same combination of event and listener will result in the listener being added multiple times. Returns emitter, so calls can be chained.
	
  - on(event, listener)

      - Adds a listener at the end of the listeners array for the specified event. No checks are made to see if the listener has already been
        added. Multiple calls passing the same combination of event and listener will result in the listener being added multiple times. Returns emitter, so calls can be chained.

	
   - once(event, listener)

      - Adds a one time listener to the event. This listener is invoked only the next time the event is fired, after which it is removed. 
        Returns emitter, so calls can be chained.

	
   - removeListener(event, listener)

       - Removes a listener from the listener array for the specified event. Caution − It changes the array indices in the listener array 
         behind the listener. removeListener will remove, at most, one instance of a listener from the listener array. If any single listener has been added multiple times to the listener array for the specified event, then removeListener must be called multiple times to remove each instance. Returns emitter, so calls can be chained.


    - removeAllListeners([event])

       - Removes all listeners, or those of the specified event. It's not a good idea to remove listeners that were added elsewhere in the 
         code, especially when it's on an emitter that you didn't create (e.g. sockets or file streams). Returns emitter, so calls can be chained.
 

     - setMaxListeners(n)

       - By default, EventEmitters will print a warning if more than 10 listeners are added for a particular event. This is a useful default
         which helps finding memory leaks. Obviously not all Emitters should be limited to 10. This function allows that to be increased. Set to zero for unlimited.


       - listeners(event)

       - Returns an array of listeners for the specified event.


    - emit(event, [arg1], [arg2], [...])

       - Execute each of the listeners in order with the supplied arguments. Returns true if the event had listeners, false otherwise.

### Class Methods


   - listenerCount(emitter, event)

       - Returns the number of listeners for a given event.