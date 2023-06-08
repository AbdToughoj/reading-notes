## Class15: Trees

### Why we use Trees:

Trees are a fundamental data structure used in computer science to organize and store data efficiently. Different types of trees, such as binary trees, binary search trees, and k-ary trees, serve specific purposes and provide different functionalities to meet varying requirements.

### What are Binary Trees, Binary Search Trees, and K-ary Trees:

- **Binary Trees**:
  Binary trees are a type of tree data structure where each node can have at most two children. They are called "binary" because each node can have either zero, one, or two children. The first node in the tree is known as the root node. Binary trees are used to represent hierarchical relationships and are the foundation for more specialized tree structures.

- **Binary Search Trees:**
  Binary search trees (BSTs) are a specific type of binary tree that incorporates an ordering property. In a BST, for any given node, all values in its left subtree are smaller than its value, and all values in its right subtree are greater. This property enables efficient searching, insertion, and deletion operations with a time complexity of O(log n). BSTs are widely used in applications where fast data retrieval is required, such as dictionaries, databases, and symbol tables.

- **K-ary Trees:**
  K-ary trees are a generalization of binary trees, allowing each node to have up to k children. The value of k determines the degree of the tree. K-ary trees are employed when more than two branches are necessary at each node. They are used in various scenarios, including representing hierarchical structures like file systems, organization charts, and decision-making processes. K-ary trees enable efficient storage and traversal of data in a structured manner.

### How we use Trees:

- Binary trees are structured by having nodes with at most two children, the left child and the right child.

- Binary search trees maintain the ordering property, ensuring that values in the left subtree are smaller and values in the right subtree are greater.

- K-ary trees generalize binary trees by allowing nodes to have up to k children, expanding the branching factor.

- Binary search trees and k-ary trees can be implemented using different algorithms and data structures, such as linked lists or arrays, to store and manipulate the tree nodes efficiently.
