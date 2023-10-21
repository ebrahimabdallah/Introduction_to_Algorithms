# Linked List 
* is a data struture in which the objects are arranged in Linear order 
* linear order is determined by the array indices.
* non-linear data structures, items don’t have to be arranged in order
* in linked list is determined by pointer in each object.
* Nodes represent those data elements, and links or pointers connect each node.
* A linked list consists of a data element known as a node
* each node consists of two fields
* 1- an address that keeps
* 2- reference to the next node
* last node contains null in its second field because it will point to no node
# The linked list types
* 1-Singly Linked List :  node has data and an address field that contains a reference to the next node
* 2-Doubly Linked List : two pointer storage blocks in the doubly linked list
* 3-Circular Linked List :the prev of head of the list point to the tail, and next pointer of tail of the list points to head.
# Array Vs.Linkedlist
| index| Linked List| Array |
| -- | -- |---|
|  |linked list don't need a contiguous memory they can grow dynamically|array need a contiguous a block of memory  |
|  | linked lists are dynamic data structures  |  arrays are static data structures |
| accessed the elements |Pointers| using index |
| Operations | Search O(n) && Deleting && Insertion | ## |

* sentinel is a dummy object that allows us to simplify boundary conditions
* The main benefit of using reference states is that it seeks to make list additions and deletions easier and simpler, as developers do not need to deal with the specificity of bounds.
