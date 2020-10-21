# Graphs

 A graph is a collection of vertices conneted by line segments called edges.
 
 __Vertex__ - Also called a node. An object with 0 or more adjacent vertices
 __Edge__ - A connection between two nodes
 __Neighbor__ - An adjacent node, connected via an edge
 __Degree__ - The number of edges connected to a vertex

 ## Directed vs Undirected

 - In an __undirected graph__, each edge is unidirected or bi-directional. The edges don't go in a specific direction in these graphs.

 - In a __directed graph__(Digraph), every edge is directed. Every node has a points to other nodes, but not necessarily the other way around. 

 ## Complete vs Connected vs Disconnected

 - A __complete graph__ is one where all the nodes are connected to all the other nodes. 

 - A __connected graph__ has nodes that all have at least one edge. A tree is a form of a connected graph

- In a __disconnected graph__, some of the vertices may not have edges

## Acyclic vs Cyclic

 - An __Acyclic graph__ is directed, and without cycles. This means that nodes can traverse through and may not end up back at themselves. A DAG or directed acyclic graph is also known as a tree

 - A __cylclic graph__ does have cycles, meaning it starts and ends at the same vertex

## Graph representation

 - An adjacency matrix is represented through a 2-dimensional array. The connected nodes are represented by 1s. 

 - A sparse graph has few connections and a dense graph has many connections

 - An adjacency list is the most common way to represent a graph, and it is a collection of the linked lists in an array

 - A weighted graph shows the nodes with numbers along the edges

 - Graphs are traversed like trees. Some graphs are cylclical, so you need to add a 'flag' to nodes that you already traversed

 - One way is breadth first. This uses a queue to help traverse. It basically looks at the first node, then nodes one edge away, then two, etc. This won't work if there are some node that can't be reached by the first node, and it won't work if there are some completely disconnected nodes. 

 - Depth first uses a stack to traverse. 

 - Graphs are very commonly used. They are used in GPS, driving directions, social networks, airline traffic, and Netflix uses them for recommendations. 