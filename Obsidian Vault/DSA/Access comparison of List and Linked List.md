
The key concepts in the selected text are about how arrays and linked lists differ in terms of how they store and access data.

**Arrays:**

- **Contiguous nature:** Elements in an array are stored next to each other in memory. This means that you can easily find the location of any element by knowing its index. For example, if you have an array of numbers and want to access the third element, you can simply calculate its memory address based on the starting address of the array and the size of each element.
- **Fast access:** Because of their contiguous nature, arrays have very fast access times. You can access any element directly by its index, which is a constant-time operation (O(1)).

**[[Linked List]]:**

- **Non-contiguous nature:** Elements in a linked list are not stored next to each other in memory. Instead, each element (called a node) contains a pointer to the next element in the list. This means that you can't directly calculate the memory address of an element based on its index.
- **Slower access:** To access an element in a linked list, you have to start at the beginning of the list and follow the pointers until you reach the desired element. This can be slow, especially if the element is near the end of the list. The time complexity for accessing an element in a linked list is directly proportional to the size of the list, which is O(n) in the worst case.

**Best and worst case time complexity:**

- **Best case:** If you're accessing the first element of a linked list, you don't need to follow any pointers, so the access time is constant (O(1)).
- **Worst case:** If you're accessing the last element of a linked list, you have to follow pointers through every element in the list, so the access time is proportional to the size of the list (O(n)).

**Average case time complexity:**

- On average, you'll have to follow pointers through half of the elements in the list to reach a specific element. This means that the average access time is also proportional to the size of the list, which is O(n).

In summary, arrays are great for random access, while linked lists are better for inserting or deleting elements at arbitrary positions.

![[Pasted image 20240906101256.png]]

