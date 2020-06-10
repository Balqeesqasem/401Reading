### Trees

#### Common Terminology:

   - Node ---->  A node is the individual item/data that makes up the data structure
   - Root ---->  The root is the first/top Node in the tree
   - Left Child ---->  The node that is positioned to the left of a root or node
   - Right Child ---->  The node that is positioned to the right of a root or node
   - Edge ---->  The edge in a tree is the link between a parent and child node
   - Leaf ---->  A leaf is a node that does not contain any children
   - Height ---->  The height of a tree is determined by the number of edges from the root to the bottommost node




###### Traversals:

        1. Depth First
        2. Breadth Firs   


   1) Depth First :
       - Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are 
         multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

                  - Pre-order: root >> left >> right
                  - In-order: left >> root >> right
                  - Post-order: left >> right >> root    


   *** The most common way to traverse through a tree is to use recursion. With these traversals, we rely on the call 
       stack to navigate back up the tree when we have reached the end of a sub-path.

###### Pre-order 
        - Pre-order means that the root has to be looked at first. In our case, looking at the root just means that we 
          output its value. 


   2) Breadth First:

         - Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. 

         - Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the
           width/breadth of the tree.


#### Trees can have any number of children per node, but Binary Trees restrict the number of children to two
 #### (hence our  left and right children).           
