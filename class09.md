### Middleware
     
     - Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions.
     - Middleware is specified on the schema level and is useful for writing plugins.

     - Mongoose has 4 types of middleware: 
            1. document middleware. (supporte validate ,save ,remove ,updateOne ,deleteOne and init )
            2. model middleware.( suport insertMany)
            3. aggregate middleware (suporte aggregate)
            4. query middleware. (supporte count ,deleteMany ,deleteOne ,find ,findOne ,findOneAndDelete ,findOneAndRemove ,findOneAndUpdate, 
                                     remove ,update ,updateOne ,updateMany).

#####   Pre
      - Pre middleware functions are executed one after another, when each middleware calls next. 

#### Use Cases

     - Middleware are useful for atomizing model logic. Here are some other ideas:

           - complex validation
           - removing dependent documents (removing a user removes all his blogposts)
           - asynchronous defaults
           - asynchronous tasks that a certain action triggers                                    

     - Post middleware
            - post middleware are executed after the hooked method and all of its pre middleware have completed.           

#### Subdocuments

     - Subdocuments are documents embedded in other documents. In Mongoose, this means you can nest schemas in other schemas. Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.    

     - Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.

###### Populate

        - Population is the process of automatically replacing the specified paths in the document with document(s) from other collection(s). We may populate a single document, multiple documents, a plain object, multiple plain objects, or all objects returned from a query.     