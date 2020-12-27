# Code 401 | Binary Trees & Binary Search Trees

## Class 15 Reading Notes

[Source: Code Fellows GitHub](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

I. Notes of Interest

- Trees are a data structure that, like linked lists or stacks and queues, connect nodes one to another.

- The structure of a tree is that of an upside down tree, with the root being the top-most node and leaves being those nodes with no continuation (i.e., connection to futher nodes).

- The metaphor of a tree breaks down with the nomenclature of the nodes between the root and the leaves: the left and right child refer to the nodes to the left or right of the root (or any node), while the "edge" is the link (or branch?) between the "parent" node and its child.

- The height of a tree refers to the number of edges between the root and the last leaf.

- There are two ways to traverse a binary tree: (1) breadth-first traversal and (2) depth-first traversal.

- Binary trees can have only two children, while trees can have as many as they'd like.

- The values in a binary tree come in no specific order.

- Big O for time when traversing a binary tree is O(n).

- Big O for space: "A “perfect” binary tree is one where every non-leaf node has exactly two children. The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree. Height can be calculated as log n, where n is the number of nodes."

- In a binary search tree (BST), "nodes are organized in a manner where all values that are smaller than the root are are placed to the left, and all values that are larger than the root are placed to the right," making searching easier, because you only have to search the half of the tree where the value is. (How does this work with strings?) Use a while loop until you either hit the match or a leaf.

- Big O for space of a search of (or insertion into) a binary search tree is 0 and for time is "O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n."

II. Teach a Concept: Using a Quiz

Q. What is the discrete unit of a tree? 
A. The node.

Q. True or false: the root of a tree is at the bottom?
A. False: it is at the top, making the leaves the bottom, so it's an inverted tree.

Q. True or false: the metaphor of the tree is used for all aspects of the data structure?
A. False: the descendent of the root is a "child," the direct forbear of a child is a parent, and what connects a parent and a child is not a branch, but an edge.

Q. How is the height of a tree calculated?
A. By counting the number of edges between the lowest leaf and the root.


