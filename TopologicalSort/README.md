
This program starts off with the topologicalSort class which receives the input (Number of vertices and edges) from the user, and the coordinates.  
The graph() method in the Graph class is the constructor for the given inputs (Vertices and edges).The time complexity of this method is O(V) where V is the amount of vertices. The method addEdge(u, v) will insert an edge to the graph with the given coordinates from the user. This method has a time complexity of O(1). The method cycles(v, visited, recStack) is a recursive method that returns true if the graph provided is a cycle. The time complexity is O(V + E), where V is the vertices and E is the edges. The isCyclic()method just uses the functionalities of the cycles function. The method topologicalSortUntil(v, visited, stack) sorts the graph in topological order using recursive functions. The time complexity is O(V + E), where V is the vertices and E is the edges. The method topologicalSorting() will perform the sorting algorithm, same time complexity. The time complexity of the overall program is O(V + E) which is based on the number of vertices and edges.

