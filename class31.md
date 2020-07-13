# combineReducers 

  - combineReducers utility to implement that behavior. It is an example of a 
    higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

  - a utility function to simplify the most common use case when writing Redux
    reducers.   

  - Each reducer technically has it’s own actions and creators. and If an action
    is dispatched with both reducers recieving it, both would respond to it. 

  - The resulting reducer calls every child reducer, and gathers their results
    into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers().

  - You may call combineReducers at any level of the reducer hierarchy. It doesn't have to happen at the top.