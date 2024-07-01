### **Task 3**

1. What is Big O notation and memory notation?
2. Why is the map fast in data structures (DS)?
3. What is the shortest path algorithm in a weighted graph?
4. Compare DFS and BFS traversal algorithms.
5. What is the difference between a binary tree, B-tree, and Red-black tree?
6. What are the types, problems, and disadvantages of HashMap?
7. What is a trie?

________________________________________________________________________________________________________________________________________________________________________________________________________________________________
### Answers :

1. **What is Big O notation and memory notation?**

**Big O Notation:**
Big O Notation is used to describe the upper bound of an algorithm's time complexity. It provides an asymptotic analysis of an algorithm's efficiency as the input size grows, focusing on the worst-case scenario. Common Big O notations include:
- \( O(1) ): Constant time
- \( O(log n) ): Logarithmic time
- \( O(n) ): Linear time
- \( O(n log n) ): Linearithmic time
- \( O(n^2) ): Quadratic time
- \( O(2^n) ): Exponential time

**Memory Notation:**
Memory notation describes the amount of memory an algorithm uses as a function of the input size. It is often denoted similarly to Big O notation (e.g., \( O(1) \), \( O(n) \), \( O(n^2) \)) and helps understand the space efficiency of an algorithm.

2. **Why is the map fast in data structures (DS)?**

Maps (or hash maps) are fast due to their underlying data structure, typically a hash table. Hash tables use a hash function to compute an index into an array of buckets or slots, from which the desired value can be found. The average time complexity for insertion, deletion, and search operations is \( O(1) \) because the hash function allows direct indexing.

3. **What is the shortest path algorithm in a weighted graph?**

The most commonly used shortest path algorithms in weighted graphs are:
- **Dijkstra's Algorithm:** Finds the shortest path from a single source to all other vertices in a graph with non-negative weights.
- **Bellman-Ford Algorithm:** Finds the shortest path from a single source to all other vertices in a graph, allowing for negative weight edges.
- **Floyd-Warshall Algorithm:** Computes shortest paths between all pairs of vertices in a graph.

4. **Compare DFS and BFS traversal algorithms.**

- **Depth-First Search (DFS):**
  - Explores as far down a branch as possible before backtracking.
  - Uses a stack (explicit or recursion).
  - Time Complexity: \( O(V + E) \) where \( V \) is the number of vertices and \( E \) is the number of edges.
  - Space Complexity: \( O(V) \) due to the stack.
  - Better for pathfinding and topological sorting.

- **Breadth-First Search (BFS):**
  - Explores all neighbors of a vertex before moving to the next level.
  - Uses a queue.
  - Time Complexity: \( O(V + E) \).
  - Space Complexity: \( O(V) \) due to the queue.
  - Better for finding the shortest path in unweighted graphs.

5. **What is the difference between a binary tree, B-tree, and Red-black tree?**

- **Binary Tree:**
  - Each node has at most two children (left and right).
  - No specific rules for balancing.

- **B-tree:**
  - A self-balancing search tree where nodes can have multiple children.
  - Used in databases and filesystems for efficient disk read/write operations.
  - Keeps data sorted and allows searches, insertions, deletions, and sequential access in logarithmic time.

- **Red-black tree:**
  - A self-balancing binary search tree.
  - Ensures that the tree remains balanced through specific properties (e.g., red and black nodes, no two red nodes in a row).
  - Time Complexity for search, insert, and delete operations is \( O(log n) \).

6. **What are the types, problems, and disadvantages of HashMap?**

- **Types:**
  - **Chaining:** Uses a list to handle collisions by storing multiple elements in the same bucket.
  - **Open Addressing:** Uses probing to find the next available slot within the array.

- **Problems:**
  - **Collisions:** Multiple keys hash to the same index, which can affect performance.
  - **Load Factor:** High load factors can degrade performance; resizing can be costly.

- **Disadvantages:**
  - **Memory Overhead:** Requires extra space for storing the hash table and handling collisions.
  - **Not Ordered:** Does not maintain the order of insertion.
  - **Complex Resizing:** Resizing the hash table involves rehashing all entries, which is time-consuming.

7. **What is a trie?**

A trie (pronounced "try") is a tree-like data structure used to store a dynamic set of strings, where keys are usually strings. It is used for efficient retrieval of keys with a common prefix. Each node represents a single character of a string, and the path from the root to a node represents a prefix of a string. Tries are commonly used in applications like autocomplete and spell check.
