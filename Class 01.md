#  Node Ecosystem, TDD, CI/CD

1. Why would you want to run JavaScript code outside of a browser?

Running JavaScript outside a browser means you are using node.js technology to execute your JavaScript code. This type of usage of javascript typically refers to backend programming where your javascript code will interact with your database and can be used to create RESTful APIs.

2. What is the difference between a module and a package?

     - Modules: - libraries for Node.js.
                - modules are in one-to-one correspondence.

     - Package: - one or more modul      

     ### In short, all modules are packages, but not all packages are meant to be used as modules.     


3. What does the node package manager do?

     - Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node.js packages in your 
       application.
    
4. Provide code snippets showing 3 different ways to export a function from a node module?

           1. exports function functionName(){return 'some written code'}
           2. module.exports = { firstFunction() , secondFunction() };
           3. modules.exports = functionName()


# NPM 
     - NPM consists of three distinct components:

             1. The website.
             2. The Command Line Interface (CLI).
             3. The registry.

