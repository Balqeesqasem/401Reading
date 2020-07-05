# Hooks are a new addition in React that lets you use state and other React features without writing a class.

# useMemoCompare :

  - This hook gives us the memoized value of an object, but instead of passing an array of dependencies
    (like with useMemo) we pass a custom compare function that gets both the previous and new value. The compare function can then compare nested properties, call object methods, or whatever else you need to do in order to determine equality. If the compare function returns true then the hook returns the old object reference.

# useAsync

 - It's generally a good practice to indicate to users the status of any async request.

# useRequireAuth

 - A common need is a way to redirect the user if they are signed out and trying to view a page that should require them
   to be authenticated. 


# useRouter
 - If you use React Router you might have noticed they recently added a number of useful hooks, specifically useParams, 
   useLocation, useHistory, and use useRouteMatch. But let's see if we can make it even simpler by wrapping them up into a single useRouter hook that exposes just the data and methods we need. In this recipe we show how easy it is to compose multiple hooks and combine their returned state into a single object. It makes a lot of sense for libraries like React Router to offer a selection of low-level hooks, as using only the hook you need can minimize unnecessary re-renders. That said, sometimes you want a simpler developer experience and custom hooks make that easy. 

# Custom Hooks
 - Custom Hooks are JavaScript functions whose names are prefixed with the word use. A custom Hook is a normal function
   but we hold them to a different standard. By adding the word used to the beginning, it lets us know that this function follows the rules of Hooks.   