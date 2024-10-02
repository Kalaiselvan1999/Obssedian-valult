## Linked Lists in Python: A Quick Overview

### What are Linked Lists?

- Linked lists are less common and less known than lists in Python.
- They are useful in specific scenarios where lists might not be efficient.
**Main 4 fundamental characteristics**
- **Head:** A pointer that stores the memory address of the first element.
- **Data:** This stores the value of the element.
- **Link/Next:** A pointer to the memory address of the next element.
- **Node:** This is the collective name of the data and link.
![[Pasted image 20240906094221.png]]

### When to Use Linked Lists

- Use linked lists when you need to:
    - Insert or delete elements efficiently at any position.
    - Store data in a linear fashion.
    - Implement algorithms like stacks, queues, and graphs.

### Using `collections.deque` for Linked Lists

- The `collections.deque` class provides a convenient way to work with linked lists in Python.
- It offers efficient operations for adding and removing elements from both ends.

### Implementing Your Own Linked Lists

- If you need more control or customization, you can create your own linked list implementation.
- This involves defining a `Node` class and a `LinkedList` class to manage the nodes.

### Other Types of Linked Lists

- There are different types of linked lists, including:
    - Singly linked lists
    - Doubly linked lists
    - Circular linked lists
- Each type has its own advantages and use cases.
-

## Linked Lists vs. Lists: A Memory Comparison

### Linked Lists

- Store elements as references to data, not the data itself.
- These references are part of the elements themselves.
- Do not require a [[Contiguous memory block]].

### Lists

- Store references to data in a contiguous memory block.
- Elements do not contain references to their data.
## Linked Lists: A Primer

**Node Structure**

- **Data:** Stores the value.
- **Next:** Points to the next node.

**Linked List Structure**

- **Head:** The first node.
- **End:** The last node, with `next` pointing to `None`.
- ![[Pasted image 20240904083851.png]]
## Queues in Python: A Brief Overview

### Key Characteristics

- **FIFO (First-In, First-Out) Principle:** Elements are added to the rear and removed from the front of the queue.
- **Front and Rear Pointers:** These pointers keep track of the first and last elements in the queue.

### Visual Representation

![[Pasted image 20240905224718.png]]

### Operations

- **Enqueue:** Adds an element to the rear of the queue.
- **Dequeue:** Removes and returns the front element of the queue.
- **Peek:** Returns the front element without removing it.  
- **Is Empty:** Checks if the queue is empty.
- **Is Full:** Checks if the queue is full (if using a fixed-size array).
## Linked Lists for Stacks: A LIFO Approach

![[Pasted image 20240905224818.png]]

**LIFO (Last-In-First-Out):**

- The last element added to a stack is the first one to be removed.
- This behavior is similar to a stack of plates where the top plate is the first one taken.

**Linked Lists and Stacks:**

- Linked lists are well-suited for implementing stacks due to their flexibility in inserting and removing elements from the beginning or end.
- The head of the linked list can represent the top of the stack.
- By adding or removing elements from the head, the LIFO behavior of a stack is achieved.

### Graphs and Adjacency Lists

- **[[/DSA/Graphs]]:** Used to represent relationships between objects or networks.
- **Directed Acyclic Graphs (DAGs):** A type of graph with directed edges and no cycles.
- **Adjacency Lists:** A common way to implement graphs, consisting of a list of linked lists.
- **Each vertex:** Stored with a collection of connected vertices.

![[Pasted image 20240905225132.png]]
## Adjacency Lists in Graphs

**Adjacency Lists** are a common representation for graphs. They consist of a list where each element represents a vertex. Each vertex is associated with a linked list containing its adjacent vertices.

- **Vertex:** A node in a graph.
- **Adjacent Vertex:** A vertex directly connected to another vertex.
- **Linked List:** A linear data structure where elements are connected by pointers.

![[Pasted image 20240905225146.png]]

```
>>> graph = {
...     1: [2, 3, None],
...     2: [4, None],
...     3: [None],
...     4: [5, 6, None],
...     5: [6, None],
...     6: [None]
... }
```

## Linked Lists for Graphs: A Concise Summary

### Key Points

- **Adjacency Lists:** A graph can be represented using adjacency lists, where each vertex is associated with a list of its adjacent vertices.
- **Linked Lists:** These lists are often implemented using linked lists, which are efficient for dynamic data structures.
- **Efficiency:** Adjacency lists, using linked lists, provide a more efficient representation of graphs compared to adjacency matrices in terms of both speed and memory.
- **Clarity:** While storing None values might seem redundant, it can improve readability and consistency in later examples.