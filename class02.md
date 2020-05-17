## This

I see how to use it as a window or refer to an object .

We have 3 JS methods of changing context :
1. Call : change the context , take multiple argument .
2. Apply : the same as Call but it's just take 2 argument .
3. Bind : return bound function and take 1 argument.

## Functional Programming (FP)

    - Do every thing in pure functions (taking input giving output).
       * Ex :
             function (name){ //input 
                 return name; // output
             }

     - We treat functions as Obj by taking input from another function or give a function as an output which is called 
        (High Order Function ) .
     - Used (Filter,Map,Reduce insisted of (for).
     - We have to deal with all data as immutable data(never change
### immutable data:
     - immutable data cause effeteness problems because i have to copy every thing every time i have to change any thing!
       So we have persistent data structures for efficient immutability which is use ( structural sharing ) it's something like tree i can add node with the new change and share with it the old one without copy every thing again and again!
     - FP libraries for JS :
         1. Mori
         2. Immutable.js


    I will read more from this link if i have time !   
    [Functional Programming](https://codewords.recurse.com/issues/one/an-introduction-to-functional-programming)

  - Name 3 advantages to Test Driven Development
           1. TDD creates a detailed specification.
           2. TDD reduces time spent on rework.
           3. You spend less time in the debugger.

 - In what case would you need to use beforeEach() or afterEach() in a test suite?
         

 - What is one downside of Test Driven Development
 - What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
 - Name a use case for a static method
- Write an example of a Higher Order function and describe the use case it solves      