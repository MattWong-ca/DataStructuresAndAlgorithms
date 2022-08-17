# Data Structures + Algorithms
## Data Structures
### Arrays
- Organizes item sequentially + contiguously
- Like objects, with a length property and data property
- Smallest footprint of any DS
  - Lookup = O(1)
  - Push = O(1)
  - Insert = O(n)
  - Delete = O(n)
- Static array (fixed in size)
  - Language like C++ allows you to manage memory, that's why it's sometimes faster 
- Dynamic array (array is copied moved over to have room for extra space)
  - Automanages memory, expands as you add more elements
- Pros: fast look ups, fast push/pop at end/start, ordered
- Cons: slow inserts/deletes when not at end of array, fixed size if using static array

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
- Singly vs Doubly
  - Singly is a fairly simple implementation compared to doubly
  - Singly requires less memory, little faster
  - Singly can't be iterated in reverse or traversed from back to front
  - Use singly when you have less memory or memory is really expensive
  

### Stacks
- Plates --> Last In First Out
- Eg. browsing history (undo)
  - Lookup = O(n)
  - Pop = O(1)
  - Push = O(1)
  - Peek = O(1)
- Very important in language specific engines (eg. JS)
- Languages modelled after stack architecture (function within function, keep popping until get to very beginning)
- Linear (can traverse sequentially)
- Can be built on top of lower-level DS like arrays/LL, therefore ensuring people only perform right operations
- Arrays allow cache locality, therefore faster since items are right next to each other
- LL have extra memory due to pointers, but have more dynamic memory

### Queues
- Lineup --> First In First Out
- Eg. Printer, Uber
  - Lookup = O(n)
  - Enqueue = O(1)
  - Dequeue = O(1) (removes 1st element)
  - Peek = O(1)
- Linear (can traverse sequentially)
- Never build with array, use LL
  - Would need to shift indexes if deleting element in array (O(n))
  - With LL, removing 1st element can be done by pointing head to 2nd element

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

### Sorting

### Searching / Binary Search
- Linear Search O(n)
  - Iterating through array to find element (best scenario is O(1) if in beginning, worst is O(n))
- Binary Search O(log(n))
  - Only if list is sorted
  - Eg. start in middle, if desired # is greater, then remove left half of numbers and search right of middle value

### Divide + Conquer

### Dynamic Programming + Memoization

### Greedy Algorithms

### Recursion

### Graph Traversal (BFS + DFS)
- Visits every element, therefore O(n)
- Breadth First Search (BFS)
  - Start with root node, then move left to right level by level
  - If you know solution is not far from root
  - If tree is very deep + solutions are rare
  - For finding shortest path
  - Pros: shortest path, closer nodes
  - Cons: more memory
- Depth First Search (DFS)
  - Follows 1 branch until it reaches leaf node, then goes back up to ancestor to find other unexplored nodes
  - DFS has lower memory requirement than BFS
  - If tree is very wide
  - If solutions are frequent but located deep
  - For determining whether path exists between 2 nodes
  - Pros: less memory (especially if you know desired value is in lower-level of tree), good at asking does path exist?
  - Cons: can get slow
  
