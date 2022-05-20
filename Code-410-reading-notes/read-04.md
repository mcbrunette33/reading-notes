##Read-04

- There are two types of Linked List - Singly and Doubly. We will be implementing a Singly Linked List in this implementation.

- Linked List - A data structure that contains nodes that links/points to the next node in the list.

- Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

- Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

- Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

- Next - Each node contains a property called Next. This property contains the reference to the next node.

- Head - The Head is a reference of type Node to the first node in a linked list.

- Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

- One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

- The biggest differentiator between arrays and linked lists is the way that they use memory in our machines. Those of us who work with dynamically typed languages like Ruby, JavaScript, or Python don’t have to think about how much memory an array uses when we write our code on a day to day basis because there are several layers of abstraction that end up with us not having to worry about memory allocation at all.

- There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.

- One way to think about Big O notation is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.

- As far as linked lists go, however, the two types of Big O equations to remember are O(1) and O(n).

- a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.