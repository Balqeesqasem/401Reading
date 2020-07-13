# Actions :

When you call an asynchronous API, there are two crucial moments in time: the moment you start the call, and the moment when you receive an answer (or a timeout).

Each of these two moments usually require a change in the application state; to do that, you need to dispatch normal actions that will be processed by reducers synchronously. Usually, for any API request you'll want to dispatch at least three different kinds of actions:

An action informing the reducers that the request began.

The reducers may handle this action by toggling an isFetching flag in the state. This way the UI knows it's time to show a spinner.

An action informing the reducers that the request finished successfully.

The reducers may handle this action by merging the new data into the state they manage and resetting isFetching. The UI would hide the spinner, and display the fetched data.

An action informing the reducers that the request failed.

The reducers may handle this action by resetting isFetching. Additionally, some reducers may want to store the error message so the UI can display it.


# Redux Thunk

   - A thunk is a function that wraps an expression to delay its evaluation.
   - is a middleware that lets you call action creators that return a function instead of an action object.
     That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the body of the function once the asynchronous operations have completed.

# React Suspense
   - Suspense is a new React feature that was announced recently at the JSConf Conference in Iceland.
   - It aims to help with handling async operations respectively in regard to CPU power and data fetching.
   - Suspense allows you to defer rendering part of your application tree until some condition is met (for example, data 
     from an endpoint or a resource is loaded).    

