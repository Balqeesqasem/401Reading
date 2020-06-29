
# setState()

   - setState() is the only legitimate way to update state after the initial state setup.
   - Update to a component state should be done using setState().
   - we can pass a function(to update state multiple times) or object to setState().

### reconciliation    
   - process is the way React updates the DOM, by making changes to the component based on the change in state.
   - process :
        * We have a search component that displays a search term.
        * That search term is currently empty.
        * The user submits a search term.
        * That term is captured and stored by setState as a value.
        * Reconciliation takes place and React notices the change in value.
        * React instructs the search component to update the value and the search term is merged in.

* React events are named using camelCase, rather than lowercase.
* With JSX you pass a function as the event handler, rather than a string.

I read about Handling Events ,Forms ,State and Lifecycle ,Components and Props and apply some codes in codepen.

