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


[1] -> [2] -> [3] -> null : Singly Linked List  (uni -direction.)
// Doubly Linked List : Bi-directional 
// nodes ?
element that has a value + has a next value (pointer) : connection
// set of nodes connected to each other:
one direction  : uni -direction.
{	value: 1,
	next: {
		value: 2, 
		next: {
			value: 3,
			next: null
		}
	}
}
// Head: first node
// Tail: last node :::::>>>> (next : null)
—————————————————————————————————————————————
BIG O Notation:
ways to describe the complexity and efficiency of algorithm (without Running it)
time and space complexity;
Time: Traversal 
Space: Storage.
O(1) : constant  —> Objects/ Hashmaps
var rawan = {name: 'rawan'};
// add another prop
rawan.email = 'email@email.com;
O(n) :Linear -> Linked List
let arr = [1, 2, 3, 4] // searching for 3 : one loop,
1- worst case scenario 
2- imagine huge number millions …
O(n log(n)) : logarithmic : divide and conquer : Binary Search Tree.
O(n^2) : two loops inside of each other <<<< — 
—————————————————————————————————————————————

            