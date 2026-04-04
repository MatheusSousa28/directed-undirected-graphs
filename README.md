**Main Content**

Hello! This repository contains an implementation of directed and undirected graphs in the C programming language, using the adjacency list method.

**What are adjacency lists?**

A graph is a data structure that represents relationships between objects, in this case, vertices.
These vertices are connected by “paths” (edges) that link one to another.

An adjacency list stores, for each vertex, all the vertices it is connected to.
This structure allows us to implement search algorithms based on the graph’s connections.

**Advantages and Disadvantages of using adjacency lists**

**Advantages:**

- Using structs makes the code more readable.

- Easier to maintain and understand.

- Relatively simple to implement.

**Disadvantages:**

- Higher memory usage compared to an adjacency matrix.

- May require more processing in certain cases.

*Alternative:* An adjacency matrix can be lighter and faster in some scenarios, but is more complex to maintain and implement.

**Search algorithms implemented**

Graphs can use different search algorithms to find the shortest path between two vertices or to determine reachability (which vertices are accessible from a given vertex). In this implementation, the directed graph uses the DFS (Depth-First Search) algorithm, which consists of going as deep as possible along a path before backtracking and exploring other paths. This algorithm is excellent for checking connectivity and detecting cycles. DFS allows access to all vertices in the graph, even those that have no connections to any other vertex, which can result in multiple trees at the end of the search; for this reason, it is said that the DFS algorithm generates a forest.

The undirected graph, on the other hand, uses the BFS (Breadth-First Search) algorithm, which works by visiting all neighbors of a vertex before moving deeper into the graph. This approach allows the determination of the shortest path (in terms of the number of edges) between the starting vertex and all other reachable vertices. Unlike DFS, BFS produces only the tree formed by the vertices that are accessible from the predefined starting vertex at the beginning of the search.

DFS and BFS algorithms are not exclusive to directed or undirected graphs; both can be applied to any type of graph. The choice between them depends on the search objective: DFS is better suited for fully exploring the graph structure and detecting cycles, while BFS is ideal for finding minimum distances and shortest paths.

[Read this in Brazilian Portuguese](README.pt.md)
