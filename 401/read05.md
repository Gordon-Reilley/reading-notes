# Linked Lists

### Important Terms

- Linked List - A data structure that contains nodes that links/points to the next node in the list.
- Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
- Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
- Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
- Next - Each node contains a property called Next. This property contains the reference to the next node.
- Head - The Head is a reference of type Node to the first node in a linked list.
- Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

### Linked list Cheat Sheet

- One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. 
- It can be helpful to think of arrays and linked lists as being similar in the way that we sequence data. In both of these structures, order matters.
- The biggest differentiator between arrays and linked lists is the way that they use memory in our machines.
- Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout. Whereas When an array is created, it needs a certain amount of memory in one contiguous block. 
- The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures.
- The starting point of the list is a reference to the first node, which is referred to as the head. Nearly all linked lists must have a head, because this is effectively the only entry point to the list and all of its elements, and without it, you wouldn’t know where to start! The end of the list isn’t a node, but rather a node that points to null, or an empty value.
- A single node is also pretty simple. It has just two parts: data, or the information that the node contains, and a reference to the next node.
- Singly linked lists are the simplest type of linked list, based solely on the fact that they only go in one direction. There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.
- Just as a node can reference its subsequent neighbor node, it can also have a reference pointer to its preceding node, too! This is what we call a doubly linked list, because there are two references contained within each node: a reference to the next node, as well as the previous node. 
- A circular linked list is a little odd in that it doesn’t end with a node pointing to a null value. Instead, it has a node that acts as the tail of the list (rather than the conventional head node), and the node after the tail node is the beginning of the list.
- Just like with an array, we can add elements and remove elements from a linked list. But unlike arrays, we don’t need to allocate memory in advance or copy and re-create our linked list, since we won’t “run out of space” the way we might with a pre-allocated array.
- A linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.
- When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.
- The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null.
- When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

### Big O Notation Cheat Sheet

- Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:

        1. Running Time (also known as time efficiency / complexity) The amount of time a function needs to complete.
        2.  Memory Space (also known as space efficiency / complexity) The amount of memory resources a function uses to store data and instructions.
- Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job.
- It specifically looks at the factors mentioned above, which we often refer to as Space and Time. In order to analyze these limiting factors, we should consider 4 Key Areas for analysis:

        1. Input Size
        2. Units of Measurement
        3. Orders of Growth
        4. Best Case, Worst Case, and Average Case
### Sources

- <https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html>
- <https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html>
- <https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d>
- <https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996>

[Back To Home](../README.md)