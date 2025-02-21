Got it! Since you already know **BFS** and **DFS**, let’s build on that and go through **all the important graph algorithms** in a structured way. I'll keep it simple and easy to remember. 🚀

---

## **🌟 Basic Concepts in Graphs**

### **1️⃣ Graph Representations**

- **Adjacency Matrix** → `O(V²)`, good for dense graphs.
- **Adjacency List** → `O(V + E)`, good for sparse graphs.

Example (Adjacency List Representation in Java):

```java
List<List<Integer>> graph = new ArrayList<>();
for (int i = 0; i < n; i++) graph.add(new ArrayList<>());
graph.get(0).add(1);
graph.get(1).add(0);
```

---

## **🔹 BFS & DFS (Recap)**

### **🔹 1. Breadth-First Search (BFS)**

- **Used for:** Shortest path (unweighted graph), Level order traversal.
- **Time Complexity:** `O(V + E)`
- **Uses:** **Queue (FIFO)**

```java
void bfs(int start, List<List<Integer>> graph) {
    Queue<Integer> queue = new LinkedList<>();
    boolean[] visited = new boolean[graph.size()];
    
    queue.add(start);
    visited[start] = true;

    while (!queue.isEmpty()) {
        int node = queue.poll();
        System.out.print(node + " ");
        
        for (int neighbor : graph.get(node)) {
            if (!visited[neighbor]) {
                queue.add(neighbor);
                visited[neighbor] = true;
            }
        }
    }
}
```

---

### **🔹 2. Depth-First Search (DFS)**

- **Used for:** Detecting cycles, Topological Sorting, Connected Components.
- **Time Complexity:** `O(V + E)`
- **Uses:** **Stack (Recursion or Explicit Stack)**

```java
void dfs(int node, List<List<Integer>> graph, boolean[] visited) {
    visited[node] = true;
    System.out.print(node + " ");
    
    for (int neighbor : graph.get(node)) {
        if (!visited[neighbor]) {
            dfs(neighbor, graph, visited);
        }
    }
}
```

---

## **🔹 Advanced Graph Algorithms**

### **🔹 3. Detecting Cycles in Graph**

- **Undirected Graph:** Use **DFS with parent check**.
- **Directed Graph:** Use **DFS + Recursion Stack**.

**Cycle Detection in Directed Graph using DFS:**

```java
boolean dfsCycle(int node, List<List<Integer>> graph, boolean[] visited, boolean[] recStack) {
    visited[node] = true;
    recStack[node] = true;

    for (int neighbor : graph.get(node)) {
        if (!visited[neighbor] && dfsCycle(neighbor, graph, visited, recStack)) return true;
        else if (recStack[neighbor]) return true; // Cycle detected
    }

    recStack[node] = false;
    return false;
}
```

---

### **🔹 4. Topological Sorting (DAG Only)**

- **Used for:** Course scheduling, Task execution order.
- **Works on:** **Directed Acyclic Graph (DAG)**.
- **Methods:**
    1. **DFS + Stack**
    2. **Kahn's Algorithm (BFS with in-degree count).**

**Topological Sort using DFS:**

```java
void topologicalSort(int node, List<List<Integer>> graph, boolean[] visited, Stack<Integer> stack) {
    visited[node] = true;
    
    for (int neighbor : graph.get(node)) {
        if (!visited[neighbor]) {
            topologicalSort(neighbor, graph, visited, stack);
        }
    }
    
    stack.push(node);
}
```

---

### **🔹 5. Shortest Path Algorithms**

**(a) Dijkstra's Algorithm (Single Source Shortest Path)**

- **Used for:** Finding shortest path from a source (Non-negative weights).
- **Uses:** **Priority Queue (Min-Heap)**
- **Time Complexity:** `O((V + E) log V)`

```java
void dijkstra(int src, List<List<int[]>> graph, int V) {
    PriorityQueue<int[]> pq = new PriorityQueue<>(Comparator.comparingInt(a -> a[1]));
    int[] dist = new int[V];
    Arrays.fill(dist, Integer.MAX_VALUE);
    dist[src] = 0;
    pq.add(new int[]{src, 0});

    while (!pq.isEmpty()) {
        int[] curr = pq.poll();
        int node = curr[0], cost = curr[1];

        for (int[] edge : graph.get(node)) {
            int neighbor = edge[0], weight = edge[1];
            if (cost + weight < dist[neighbor]) {
                dist[neighbor] = cost + weight;
                pq.add(new int[]{neighbor, dist[neighbor]});
            }
        }
    }
}
```

---

**(b) Bellman-Ford Algorithm**

- **Used for:** Graphs with **negative weights**.
- **Time Complexity:** `O(VE)`
- **Detects negative cycles**.

```java
void bellmanFord(int src, List<int[]> edges, int V) {
    int[] dist = new int[V];
    Arrays.fill(dist, Integer.MAX_VALUE);
    dist[src] = 0;

    for (int i = 0; i < V - 1; i++) {
        for (int[] edge : edges) {
            int u = edge[0], v = edge[1], w = edge[2];
            if (dist[u] != Integer.MAX_VALUE && dist[u] + w < dist[v]) {
                dist[v] = dist[u] + w;
            }
        }
    }
}
```

---

### **🔹 6. Minimum Spanning Tree (MST)**

- **Finds the minimum cost to connect all nodes in an undirected graph.**
- **Algorithms:**
    1. **Kruskal’s Algorithm** → Uses **Sorting + Union-Find (DSU)**.
    2. **Prim’s Algorithm** → Uses **Priority Queue (Min-Heap)**.

**Kruskal’s Algorithm (Union-Find Approach)**

```java
int kruskalMST(int V, List<int[]> edges) {
    Collections.sort(edges, Comparator.comparingInt(a -> a[2])); // Sort by weight
    UnionFind uf = new UnionFind(V);
    int mstWeight = 0, count = 0;

    for (int[] edge : edges) {
        if (uf.union(edge[0], edge[1])) { // If adding this edge does not create a cycle
            mstWeight += edge[2];
            count++;
            if (count == V - 1) break; // MST formed
        }
    }
    return mstWeight;
}
```

---

### **🔹 7. Strongly Connected Components (SCC)**

- **Used for:** Finding strongly connected subgraphs in a **directed graph**.
- **Algorithms:**
    1. **Kosaraju’s Algorithm** → Uses **DFS twice**.
    2. **Tarjan’s Algorithm** → Uses **DFS + Low Link Values**.

---

### **🔹 8. Floyd-Warshall Algorithm**

- **Used for:** All-pairs shortest paths.
- **Time Complexity:** `O(V³)`.
- **Dynamic Programming Approach.**

```java
void floydWarshall(int[][] dist, int V) {
    for (int k = 0; k < V; k++) {
        for (int i = 0; i < V; i++) {
            for (int j = 0; j < V; j++) {
                dist[i][j] = Math.min(dist[i][j], dist[i][k] + dist[k][j]);
            }
        }
    }
}
```

---

## **🔹 Summary**

|Algorithm|Use Case|
|---|---|
|**BFS**|Shortest path in unweighted graph|
|**DFS**|Cycle detection, Connected components|
|**Dijkstra**|Shortest path (Non-negative weights)|
|**Bellman-Ford**|Negative weights, Detect negative cycles|
|**Kruskal / Prim**|Minimum Spanning Tree|
|**Topological Sort**|DAG-based task ordering|
|**Kosaraju / Tarjan**|Strongly Connected Components|

---

This should help you **revise graphs quickly**! Let me know if you want **detailed explanations on any topic. 🚀**