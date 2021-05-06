# Reading 35 Notes

[Home](README.md)

# Graphs

## What is a graph?
Graphs are non-linear data structures that can be thought of as a collection of vertices (nodes) usually connected by line segments called edges.

### Terminology when working with Graphs:
1. *Vertex*: This is also called a "node". It's a data object that can have none or moreadjacent vertices.
2. *Edge*: A connection between two nodes.
3. *Neighbor*: Neighbors of a node are the adjacent nodes.
4. *Degree*: The degree of a vertex is the number of how many edges are connected to that vertex.

## Directed vs Undirected Graphs
### Undirected Graphs
Undirected Graphs are where each edge is undirected or bi-directional, meaning that the undirected graph doesn't move in any direction.

In the example below you can see that Node *C* is connected to Nodes *A, E and B*, There aren't any directions given to point to a specific vertex. This connection is bi-directional.
This graph has 6 vertices and 7 undirected edges.
[UndirectedGraph.png](../assets/UndirectedGraph.png)

### Directed Graphs (Digraph)
Directed Graphs are also called Digraphs which is a graph where every edge is directed. Unlike the undirected graphs, a Digraph has direction. Each of the nodes are directed at another with a speicifc requirement to what node should be reffered to next. In the example below, The Digraph has arrows pointing to specific nodes.
This graph has 6 vertices and 8 directed edges.
[DirectedGraph.png](../assets/DirectedGraph.png)

## Complete, Connected, Disconnected graphs
### Complete Graphs 
These graphs are when all nodes are connected to eachother.

### Connected Graphs
These graphs are when all of the vertices or nodes have at least one edge.

### Disconnected
These graphs are where some vertices may not have edges.


