# Data Structures + Algorithms
## Data Structures
### Arrays
- Organizes item sequentially + contiguously
- Smallest footprint of any DS
  - Lookup = O(1)
  - Push = O(1)
  - Insert = O(n)
  - Delete = O(n)

### Linked Lists
- Made up of nodes (value + pointer to next element)
- Tail node points to null
- Easier to traverse and insert in LL than in array
- Can have sorted data, unlike hash table
- Big-O
  - Prepend = O(1) (don't have to loop through anything just had references to head/tail and re-assigned values)
  - Append = O(1)
  - Lookup = O(n)
  - Insert = O(n)
  - Delete = O(n)

### Stacks / Queues

### Sets

### Hashes / Maps / Dictionaries
- Maps `keys` to specific values

### Trees
- Root --> Parent --> Child --> Leaf --> Sibling
- Ex: Facebook comments, HTML pages
- LL is type of tree but with single path
- Binary Tree
  - Each node can only have 0 1 or 2 nodes
  - Each child can only have 1 parent
  - Perfect Binary Tree: all nodes are full
  - Full Binary Tree: only 0 or 2 children
- Binary Search Tree
  - Lookup = O(logN)
  - Insert = O(logN)
  - Delete = O(logN)

### Heaps

### Graphs

## Algorithms
### Big-O Analysis
- Iterating through array is `O(n)` (linear)
- Taking 1st item of array is `O(1)` (constant)

### Sorting / Searching / Binary Search

### Divide + Conquer

### Dynamic Programming + Memoization

### Greedy Algorithms

### Recursion

### Graph Traversal (BFS + DFS)
