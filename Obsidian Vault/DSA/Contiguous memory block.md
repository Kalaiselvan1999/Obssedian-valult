**An array is a data structure that is used to store elements in contiguous memory locations. What this essentially means, is that each element is stored in a memory location adjacent to one another. Additionally, the size of an array is unchangeable and is declared beforehand**

The key concept in the selection "lists use a contiguous memory block to store references to their data" is that lists in Python are stored in a specific, ordered way in the computer's memory. This is different from other data structures like dictionaries, which are not stored in a specific order.

**Contiguous memory block:** This means that the elements of a list are stored one after another in a continuous block of memory. Think of it like a row of houses on a street, where each house is next to the other.

**References:** In Python, when you create a list, the list itself doesn't store the actual data. Instead, it stores references to the data. A reference is like a pointer or address that tells the computer where to find the data. So, each element in a list is actually a reference to the object it points to.

**Example:**

Python

```
my_list = [1, 2, 3]
```

In this example, `my_list` is a list that contains three elements: 1, 2, and 3. These elements are stored in a contiguous memory block, and `my_list` stores references to each of these elements. So, when you access the first element of the list, Python follows the reference to find the actual value, which is 1.

**Why is this important?**

The fact that lists use a contiguous memory block has several implications:

- **Efficient access:** Because the elements are stored in a specific order, it's very efficient to access elements by their index (e.g., `my_list[0]` to access the first element).
- **Insertion and deletion:** While it's relatively efficient to insert or delete elements at the beginning or end of a list, it can be less efficient to insert or delete elements in the middle, as this requires shifting elements in the memory block.
- **Memory usage:** Lists can be memory-efficient, especially when compared to other data structures like dictionaries.

In summary, lists in Python are stored in a contiguous memory block, and they store references to the data they contain. This has implications for how efficiently elements can be accessed and inserted or deleted, as well as how much memory is used.


# Linked list

The selected statement, "linked lists store references as part of their own elements," means that each item in a linked list doesn't just contain its own data, but also a pointer (or reference) to the next item in the list. This is what makes linked lists different from arrays.

Here's a simple example:

Imagine a linked list representing a grocery list. Each item in the list is a node. The first node might contain the item "milk" and a reference to the next node. The next node might contain "eggs" and a reference to the next node, and so on. The last node would contain "bread" and a reference to None, indicating that there are no more items in the list.

This structure allows linked lists to be dynamic, meaning they can grow or shrink as needed. For example, if you want to add "butter" to the grocery list, you simply create a new node for "butter" and update the reference in the "bread" node to point to the new "butter" node.

In summary, linked lists are like a chain of nodes, where each node holds both data and a pointer to the next node in the chain. This structure makes linked lists flexible and efficient for certain operations, especially those involving insertions and deletions.