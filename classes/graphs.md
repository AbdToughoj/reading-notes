## Class 37: Graphs

A graph is a fundamental data structure in computer science that represents a collection of interconnected objects, known as nodes, and the relationships between these nodes, known as edges. Graphs are used to model a wide range of real-world scenarios and problems, including social networks, transportation systems, computer networks, recommendation systems, and more.

Graphs are particularly versatile because they can represent both simple relationships and complex connections that may not conform to a linear structure. They are composed of two main components:

- **Nodes (Vertices):** Nodes are individual entities in the graph that can represent anything, such as people, locations, web pages, or concepts. Each node can store data, attributes, or any other information relevant to the application. Nodes are often depicted as circles or points in visual representations of graphs.

- **Edges (Links):** Edges are the connections between nodes that indicate a relationship or interaction. Edges can be directed or undirected, depending on whether the relationship between nodes has a specific direction. In a directed edge, there's a starting node and an ending node, indicating a one-way relationship. In an undirected edge, the relationship is symmetric, with no distinct direction. Edges can also be weighted to represent the strength, distance, cost, or any other relevant metric of the relationship.

Graphs can be categorized into various types based on their characteristics:

- **Directed vs. Undirected Graphs:** In directed graphs (also known as digraphs), edges have a direction, while in undirected graphs, edges have no specific direction.

- **Weighted vs. Unweighted Graphs:** In weighted graphs, edges have associated weights or values that convey additional information about the relationships, while unweighted graphs have no such values.

- **Cyclic vs. Acyclic Graphs:** A cyclic graph contains at least one cycle, which is a sequence of nodes and edges that starts and ends at the same node. An acyclic graph has no cycles.

- **Connected vs. Disconnected Graphs:** A connected graph has a path between any two nodes, while a disconnected graph has components that are not reachable from each other.

- **Sparse vs. Dense Graphs:** A sparse graph has relatively few edges compared to the number of nodes, while a dense graph has a relatively large number of edges.
