# Context
    - Context provides a way to pass data through the component tree without having to pass props down manually at every
      level.

    - Context is designed to share data that can be considered “global” for a tree of React components, such as the
      current authenticated user, theme, or preferred language.

    - Context is primarily used when some data needs to be accessible by many components at different nesting levels, 
      Apply it sparingly because it makes component reuse more difficult.  

    - If you only want to avoid passing some props through many levels, component composition is often a simpler 
      solution than context.    

# Snackbars :

      - They are small notifications that show up on the screen when a user performs an action.
      - Asnackbars fit perfectly on the ‘low priority’ end of that spectrum.