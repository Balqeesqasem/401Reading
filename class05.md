# Linked Lists

  - Linked Lists : sequence of Nodes that are connected/linked to each other.
  - linked lists are linear data structures.
  - linked lists are dynamic data structures.
  - The most defining feature of a Linked List is that each Node references the next Node in the link.
  - A linked list is made up of a series of nodes.
  - Node :  Nodes are the individual items/links that live in a linked list. Each node contains the data for each link and a reference to the next node.
  - A node only knows about what data it contains, and who its neighbor is.

             * Head Node : The first node in link list.
             * current Node : that is currently being looked at.
             * Next Node : the reference to the next node.
             

  - There are two types of Linked List : 
                                          * Singly : A Singly linked list means that there is only one reference, and
                                                    the reference points to the next node in a linked list.
                                                    
                                          * Doubly : A Doubly linked list means that there is a reference to both the 
                                                     Next and Previous node.



#### Traversal 

      In Traversal we are not able to use For loop or forEach because  we will depend on the Next value  in each node to guide us where the next reference is pointing , but it's allow as to use the While loop in this way we will keep check if the next node not null and wen we reach the node that is null a NullReferenceException  gets thrown and our program will crash/end.


            