Graph Traversal in C: DFS & BFS

This repository contains a C program that demonstrates two fundamental graph traversal algorithms:

Depth-First Search (DFS)
Breadth-First Search (BFS)
Both algorithms are implemented using an adjacency list representation for efficiency.

Program Workflow
1. The program asks the user to provide:

  . Number of vertices
  . Number of edges
   .Each edge as a pair of connected vertices


2. The graph is stored as an undirected adjacency list
3. The user enters a starting node
4. The program performs both traversals from the starting node:
  . DFS (using recursion)
  . BFS (using a queue)
5. The order of visited nodes is displayed for each algorithm


Sample Run

Input
Vertices: 7
Edges: 6
Enter edges:
1 2
1 3
2 4
2 5
3 6
3 7
Start vertex: 1

Output
DFS starting at 1: 1 2 4 5 3 6 7
BFS starting at 1: 1 2 3 4 5 6 7

Graph Structure
      1
      / \
     2   3
    / \  / \
   4  5 6  7

Algorithm Insights

Depth-First Search (DFS)
 .Explores one branch fully before moving to another
 .Implemented with recursion (can also use a stack)
 .Good for exploring deep paths and detecting cycles

Breadth-First Search (BFS)
.Explores all neighbors first before going deeper
.Implemented with a queue
.Useful for shortest path problems in unweighted graphs


 Complexity Analysis
For a graph with V vertices and E edges:
Algorithm    Time Complexity   Space Complexity
DFS              O(V + E)        O(V)
BFS              O(V + E)        O(V)
Both visit every vertex and every edge exactly once.

Real-Life Applications
.DFS
  .Solving puzzles and mazes
  .Topological sorting in scheduling problems
  .Checking graph connectivity

.BFS
  .Finding shortest paths in maps/networks
  .Social network friend suggestions
  .Web crawlers exploring websites

How to Compile and Run
Requirements
  .GCC compiler
  .Linux, macOS, or Windows with a C environment

Steps
# Compile
gcc graph.c -o graph
# Run
./graph
