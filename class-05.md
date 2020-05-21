# Linked Lists
A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.
 
# What does it look like 
![Image](img/link3.jpeg)

# Big O

* The Big O of time for **Includes** would be O(n). 
This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

* The Big O of space for **Includes** would be O(1).
 This is because there is no additional space being used than what is already given to us with the linked list input.

# Prerequisites

When constructing your code, a few things to keep in mind.

1. When making your Node class, consider requiring a value to be passed in to require that each node has a value.

2. When making a Linked List, you may want to require that at least one node gets passed in upon instantiation. This first node is what your Head and Current will point too.

# Linear data structures

One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.

- In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

# Memory management


![Image](img/link2.jpeg)
