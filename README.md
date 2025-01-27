# BFS
Simple Python implementation of Breadth-First Search (BFS) algorithm for graph traversal.<br>
- BFS is an efficient algorithm for finding the shortest path between two nodes in an unweighted graph.
BreakDown of the code 
**1) Initialization:<br>**
- **graph:** This dictionary represents the graph. Keys are nodes, and their corresponding values are lists of their adjacent nodes.<br>
- **start:** This variable stores the starting node for the BFS traversal.<br>
- **queue:** A deque (double-ended queue) is used to efficiently add and remove nodes during the traversal. Initially, it contains only the start node.<br>
- **visited:** A set is used to keep track of nodes that have already been visited, preventing cycles and ensuring each node is explored only once.<br>

**2) Breadth-First Search (BFS) Loop:**<br>
- The **while queue loop** continues as long as there are nodes to explore in the queue.<br>
- **node = queue.popleft() :** In each iteration, the node at the front of the queue is dequeued (removed from the front) and processed.<br>
- **print(node, end=" ") :** The current node is printed. (This is for visualization and may not be part of the core BFS algorithm)<br>
- **for neighbor in graph[node]:** The code iterates through each neighbor of the current node.<br>
    - **if neighbor not in visited:** If the neighbor has not been visited before:<br>
    - **visited.add(neighbor):** The neighbor is added to the visited set.<br>
    - **queue.append(neighbor):** The neighbor is added to the end of the queue for exploration later.<br>

    ****OUTPUT** :**
  A B C D E F <br><br>
  MADE BY - SWAGNIK SHIT <br>
  REG NO. - 2301292134
