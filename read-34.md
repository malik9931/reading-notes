## Graphs

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* Edge - An edge is a connection between two nodes.
* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* Degree - The degree of a vertex is the number of edges connected to that vertex.


Undirected Graphs: each edge is undirected or bi-directional
![fd](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

Directed Graphs (Digraph): every edge is directed
![ds](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)


###### Depends on how connected the graphs are to other node/vertices.

Complete Graphs: all nodes are connected to all other nodes
![xz](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/CompleteGraph.PNG)


Connected: all of vertices/nodes have at least one edge.
![dsl](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/ConnectedGraph.PNG)

Disconnected: some vertices may not have edges.
![ds](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DisconnectedGraph.PNG)



* Acyclic graph - is a directed graph without cycles. Cycle is when a node can be traversed through and potentially end up back at itself.
  * Cyclic graph - is a graph that has cycles. Cycle is defined as a path of a positive length that starts and ends at the same vertex.
  * Adjacency matrix - is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix
  * Sparse graph - is when there are very few connections
  * Dense graph - is when there are many connections
  * Adjacency list is the most common way to represent graphs, and is a collection of linked lists or array that lists all of the other vertices that are connected. Also, make it easy to view if one vertices connects to another.
