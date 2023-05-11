## Class 05: Linked Lists

### **Big O: Analysis of Algorithm Efficiency**

Big O notation is a mathematical notation used to describe the efficiency of an algorithm or a function in terms of its worst-case time complexity. It measures how the running time of an algorithm grows as the input size increases.

The "O" in Big O stands for "order of" and is used to represent the upper bound of the time complexity of an algorithm. The time complexity is usually expressed as a function of the input size, and the Big O notation provides a way to simplify this function by ignoring the constant factors and lower order terms.

For example, if an algorithm has a time complexity of O(n), it means that its running time grows linearly with the input size. If the input size doubles, the running time of the algorithm will also double.

Big O notation is an important tool in computer science because it allows us to compare the efficiency of different algorithms and choose the most appropriate one for a given problem. It also helps us to identify performance bottlenecks in our code and optimize them for better performance.

### **Linked Lists**

Let's say we want to create a Linked List to store a list of songs that we have in a playlist. We'll use the following songs in our example: "Bohemian Rhapsody" by Queen, "Stairway to Heaven" by Led Zeppelin, and "Hotel California" by The Eagles.

Step 1: Creating the first node
The first node in the Linked List will represent the first song on our playlist, "Bohemian Rhapsody." We create the node by defining a class in our code with two properties: "data" and "next." The "data" property will hold the title of the song, and the "next" property will hold a reference to the next node in the list. Since this is the first node, the "next" property will be set to None.

Step 2: Creating the second node
The second node in the Linked List will represent the second song on our playlist, "Stairway to Heaven." We create the node in the same way as the first node, and set its "data" property to the title of the song. However, since this is not the first node in the list, we need to set the "next" property of the first node to point to this second node.

Step 3: Creating the third node
The third and final node in the Linked List will represent the third song on our playlist, "Hotel California." We create the node in the same way as the first two nodes, and set its "data" property to the title of the song. Since this is not the first node, we need to set the "next" property of the second node to point to this third node.

Step 4: Traversing the Linked List
Now that we have created our Linked List, we can traverse it to access the data that we have stored. We start at the first node (the head of the list) and follow the "next" references from node to node until we reach the last node (the tail of the list). We can then access the data stored in each node (in this case, the title of each song) by referencing the "data" property of each node.

Why use a Linked List?

Linked Lists are useful when you need to store a collection of data that needs to be easily accessible and modifiable. They are particularly useful when you need to add or remove items from the list frequently, since adding or removing an item from a Linked List can be done in constant time (O(1)).

What are the advantages of a Linked List?

One advantage of a Linked List is that it allows for constant-time insertions and deletions, since you only need to update the "next" references of a few nodes to add or remove an item. Additionally, Linked Lists can be used to implement more complex data structures, such as stacks, queues, and hash tables.
