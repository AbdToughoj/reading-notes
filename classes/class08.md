## Class 08 : Stacks and Queues

In Python, stacks and queues are data structures that allow you to organize and manipulate data in a specific order. They are both abstract data types and can be implemented using various underlying data structures, such as lists or linked lists.

1)Stack:

- A stack is a Last-In-First-Out (LIFO) data structure, which means that the last element added to the stack is the first one to be removed.
  \*In Python, you can implement a stack using a list. The list class provides built-in methods such as append() and pop() that can be used to simulate the stack behavior.
- To push an item onto the stack, you can use the append() method to add it to the end of the list.
- To pop an item from the stack, you can use the pop() method without passing any index, which removes and returns the last item in the list.
- Here's an example of a simple stack implementation using a list:

```
stack = []

# Push items onto the stack
stack.append(1)
stack.append(2)
stack.append(3)

# Pop items from the stack
item = stack.pop()  # item = 3
item = stack.pop()  # item = 2
```

2)Queue:

- A queue is a First-In-First-Out (FIFO) data structure, which means that the first element added to the queue is the first one to be removed.
- In Python, you can implement a queue using a list as well. However, using a list for a queue can be inefficient because removing an element from the beginning of a list requires shifting all other elements.
- Alternatively, you can use the collections.deque class from the Python standard library, which provides an optimized implementation of a queue.
- To enqueue an item into the queue, you can use the append() method of deque.
- To dequeue an item from the queue, you can use the popleft() method of deque, which removes and returns the leftmost item in the deque.
- Here's an example of a queue implementation using collections.deque:

```
from collections import deque

queue = deque()

# Enqueue items into the queue
queue.append(1)
queue.append(2)
queue.append(3)

# Dequeue items from the queue
item = queue.popleft()  # item = 1
item = queue.popleft()  # item = 2
```

Stacks and queues are commonly used in various algorithms and programming problems. Stacks are often used for backtracking, function call stack management, and evaluating expressions, while queues are useful for managing tasks, handling events, and implementing breadth-first search algorithms, among other applications.
