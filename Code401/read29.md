# Graphs


**A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.**


## TERMS:

* Vertex : A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.

* Edge : An edge is a connection between two nodes.

* Neighbor : The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.

* Degree : The degree of a vertex is the number of edges connected to that vertex.

## Operations

**The basic operations provided by a graph data structure G usually include:**

- adjacent(G, x, y): tests whether there is an edge from the vertex x to the vertex y;

- neighbors(G, x): lists all vertices y such that there is an edge from the vertex x to the vertex y;

- add_vertex(G, x): adds the vertex x, if it is not there;

- remove_vertex(G, x): removes the vertex x, if it is there;

- add_edge(G, x, y): adds the edge from the vertex x to the vertex y, if it is not there.

- remove_edge(G, x, y): removes the edge from the vertex x to the vertex y, if it is there.

- get_vertex_value(G, x): returns the value associated with the vertex x.

- set_vertex_value(G, x, v): sets the value associated with the vertex x to v.

- Structures that associate values to the edges usually also provide

