# Linked Lists

[Big o: Analysis of Algorithm Efficiency](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)

Big O(oh) notation is used to describe the efficiency of an algorithm or function. 

**Below are the two factors to consider with using Big o notation**

**Running Time** - The amount of time a function needs to complete.

**Memory Space** - The amount of memory resources a function uses to store data and instructions.

**Input Size** - Refers to the size of the parameter values that are read by the algorithm.

Consider these three factors in order to quantify the **Running Time** :

- time in milliseconds
-  number of operations executed
- number of “Basic Operations” executed

Consider these factors in order to quantify the **Memory Space** :

- amount of space needed hold the code for the algorithm
-  space needed to hold the input data
- space needed for the output data
- pace needed to hold working space during the calculation

**Big O** describes the Worst Case for algorithm efficiency. The Order of Growth used represents the upper bounds of Time and Space.

**Big Omega**: This notation describes the Best Case for a given algorithm.
**Big Theta**: The typical or random case used for analysis of algorithm efficiency.


[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

A Linked List is a sequence of Nodes that are connected/linked to each other. Each Node references the next Node in the link. 
The two types of linked lists -are **Singly** and **Doubly**.


![Linked List](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

[What’s a Linked List, Anyway pt1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

![Linear vs non](https://miro.medium.com/max/1400/1*Xokk6XOjWyIGCBujkJsCzQ.jpeg)

There is a sequence and an order to how they are constructed and traversed known as the Linear data structure. 

![static and dynamic](https://miro.medium.com/max/1400/1*G43FVT5xJ1n1QDKVNZUxXQ.jpeg)

**Arrays** are static data structures. Linked lists are dynamic data structures. A static data structure needs all of its resources to be allocated when the structure is created. However, a dynamic data structure can shrink and grow in memory

[What’s a Linked List, Anyway pt2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

        "There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs."

![space and time](https://miro.medium.com/max/1400/1*FC0XX0-9Vx7yCS0dTS2Zrw.jpeg)

#### Three steps to grow a linked list

1. First, we find the head node of the linked list.
1. Next, we’ll make our new node, and set its pointer to the current first node of the list.
1. Lastly, we rearrange our head node’s pointer to point at our new node.

        "a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element."


![side by side comparison of Arrays and Linked Lists](https://miro.medium.com/max/1400/1*cUehR5S18XSoVLaPNfNzlA.jpeg)


