# Code 401 | Data Types: Linked Lists

## Class 05 Reading Notes

### [Linked Lists by CF](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

I. Definitions

- Nodes: an item in a list that contains data for the link.
- Nodes linked to each other in sequence.
- The sequence is its definiing characteristic: linear.
- Next = property that refers to the next node; head = refers to the first node in a link.

II. Types

- Singly linked: one reference, which points to the following node.
- Doubly linked: two references, one forward and one backward, sequentially.
- Circularly linked lists: the tail points to the head.

III. Traversal

- While loop; use the next key-value pair of the current node.

### ["What's a Linked List, Anyway?: Part 1"](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

I. Data Type = linear structure = sequence + order of traversal, e.g. arrays

II. Memory: Array vs Linked List

- An array needs memory to be free all in one place, contiguous blocks and, as a static structure, it requires all of its allocated resources at creation.
- A linked list can be created in various places in memory that aren't necessarily next to each other and, as a dynamic structure, will use only the memory needed at the time for the task. 

III. Structure

- Start = head = a reference to node 1.
- End = node that points to null.
- A node = two parts = the data it contains and a reference to the next node.
- Concept: "A node only knows about what data it contains, and who its neighbor is."

### ["What's a Linked List, Anyway?: Part 2"](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

I. Big O = a method for evaluating the efficiency of an algorithm.

- time to run per number of elements passed in.
- how quickly an algorithm's runtime grows with the increase of the number of input elements.
- O equals order, i.e., magnitude(?), with n as the number of inputs.

II. Big O and Linked Lists

- O(1) = constant
- 0(n) = linear growth
- (0(n-squared) = exponential) => to be avoided

III. Adding to a Linked List from the Beginning

- Rearrange pointers
- The steps are (1) find the head, (2) make new node and point it at the first node, and (3) reassign the head to point to the new node.
- adding a node to the front of a linked list has a Big 0 of 0(1), because it's not dependent on the length of the list.

IV. Adding to a Linked List from the End

- Same steps as above, referencing correctly
- Difference: to find the last node, you have to traverse the whole list = time, which is dependent on the number of items in the list.
- O(n).

V. Conclusion

- Good for adding/removing elements and when you don't know the size of the list (while an array is good when you know the size of the list). 
- Bad for searching for a single element (while an array would be good for this).

[<--back](401week1.md)

[<--home-->](../../README.md)
