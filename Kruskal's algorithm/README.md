The find() method takes in an array of integers representing the parent of each node and an integer representing the node and it returns the root of the set in which the node belongs. It uses recursion to traverse up the tree to find the root.
The union() method takes in an array of integers representing the parent of each node, and two integers representing the nodes and it merges the sets of the two nodes by setting the parent of the first node's set to the second node's set.
The kruskal() method takes in a 2D array representing the graph where the value at each cell represents the weight of the edge between the corresponding nodes. It starts by initializing an array of integers representing the parent of each node and filling it with -1, representing that initially each node is in its own set. It then creates a queue of edges, where each edge is represented by an object of the Edge class, and adds all the edges from the graph to the queue. Then it sorts the edges based on their weight in ascending order. The method then repeatedly selects the edge with the smallest weight that doesn't form a cycle and adds it to the minimum spanning tree, updating the parent array for the nodes involved in the edge.
The program uses Kruskal's algorithm to find the minimum spanning tree of a weighted graph. It starts by creating a queue of edges, sorting them based on their weight, and then repeatedly selecting the edge with the smallest weight that doesn't form a cycle, adding it to the minimum spanning tree, and updating the parent array for the nodes involved in the edge. When the number of edges in the minimum spanning tree is equal to V-1(V represents the number of vertices in the graph), the algorithm stops.

The program also defines an Edge class which is used to represent an edge in the graph, it has 3 fields, src, dest and weight which represents the source, destination and weight of the edge respectively.