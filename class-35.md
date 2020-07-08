# Graphs

## Common terminologies

1. Vertex: A node data object that can have zero or more adjacent vertices.

2. Edge: connection between 2 nodes.

3. Neighbor: nodes connected via edge.

4. Degree: how many edges it got.

## Directed vs Undirected

### Undirected Graphs

* It's a graph where each edge is undirected or bi-directional.

* This occures when a connected node edge has no directions so it's connected to all of them.

### Directed Graphs (Digraph)

* It's a graph where every edge is directed.

* Each node is directed at another node.

## Complete vs Connected vs Disconnected

* Types of graphs depend on how connected the graphs are to other vertices.

### Complete Graphs

* A graph where all nodes are connected to eachother.

### Connected

* A graph where all the nodes have at least one edge.

* A tree is a form of connected graphs.

### Disconnected

* A graph where some nodes may not have edges.

* Solo nodes or edges are called ***islands***.

## Acyclic vs Cyclic

### Acyclic Graph (DAG)

* It's a directed graph without cycles.

* Cycle is when a node can be traveresd and end at itself.

* Tree's are DAG's.

### Cyclic Graphs

* It has cycles.

* Cycle is a path of a positive length that starts and ends at the same vertex.

## Graph Representation

Graphs are represented by:

1. Adjacency Matrix

2. Adjacency List

### Adjacency Matrix

* It's a two dimensional array (matrix), it's a binary matrix of n*n

* If a value is 1, then that means its connected, if 0 its not.

### Adjacency List

* It's a collection of linked lists or array that lists all other vertices.

## Traversals

* Traversal is similar to a tree.

### Breadth First

* Start at a specific node, it's similar to trees exept that graphs can have cycles.

* Breadth first will go in as: 
1. Enqueue the start node into the queue.
2. While loop that runs while node still has nodes.
3. Dequeue first node from queue.

### Depth first

* We use stack here

1. Push root node into the stack.
2. While loop that runs while node still has nodes.
3. Peek at top node, if it has unvisited children mark top as visited then push any unvisited into the stack.


## Real World Uses of Graphs

1. Maps and GPS.
2. Driving directions.
3. Social networks.