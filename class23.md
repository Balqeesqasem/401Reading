# Component Composition :

  - React's composition model we use it for example to re-use component code is tabs which show different content when selected. This guide will start with a set of tabs that re-use no code whatsoever and build specialized components, container components, and a combination of both to achieve re-use through composition.

  - All React components have a special children prop so that consumers can pass components directly by nesting them inside the jsx. This prop can be used by a tab content component to accept the actual content without needing to know anything else about it.

# Containment
  - Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.  

# Specialization
 - Sometimes we think about components as being “special cases” of other components. For example, we might say that a WelcomeDialog is a special case of Dialog.  


# Inheritance 
 
  - Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way. Remember that components may accept arbitrary props, including primitive values, React elements, or functions.

  - If you want to reuse non-UI functionality between components, we suggest extracting it into a separate JavaScript module. The components may import it and use that function, object, or a class, without extending it.