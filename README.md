# Minimum Spanning Tree (MST) Algorithms

This C++ implementation demonstrates two fundamental algorithms for finding Minimum Spanning Trees (MST) in graphs: **Prim's algorithm** and **Kruskal's algorithm**.

## Features
- Implementation of Prim's MST algorithm (O(E log V) time complexity)
- Implementation of Kruskal's MST algorithm (O(E log E) time complexity)
- Graph representation using adjacency lists
- Disjoint Set Union (DSU) data structure for Kruskal's algorithm
- Priority queue optimization for Prim's algorithm

## Code Structure
```plaintext
pk.cpp
├── Graph struct
│   ├── Constructor (V vertices, E edges)
│   ├── primMST() - Prim's algorithm implementation
│   └── kruskalMST() - Kruskal's algorithm implementation
│       ├── find() - DSU find operation
│       └── Union() - DSU union operation
└── main() - Example usage with sample graph

Requirements
C++11 or later

Standard Template Library (STL)

git clone https://github.com/your-username/repo-name.git

g++ pk.cpp -o mst -std=c++11

Sample Output
The program will output both MSTs:

plaintext
Copy
Prim's MST:
0 - 1
1 - 2
0 - 3
1 - 4

Kruskal's MST:
0 - 1
1 - 2
1 - 4
0 - 3


Graph Example
The default graph (V=5, E=7) is:


(0)---2---(1)---3---(2)
 | \     / |       / 
 6  8   5  7     /
 |   \ /   |   /
(3)---9---(4)


To use your own graph:

Modify the number of vertices (V) and edges (E)

Update the edges array in main():

cpp
Copy
graph.edges[0] = {src, dest, weight};
// Add more edges...
Complexity Analysis
Algorithm	Time Complexity	Space Complexity
Prim's	O(E log V)	O(V + E)
Kruskal's	O(E log E)	O(V)
Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

License
MIT
