# 🚀 Graph Cycle Detection using DFS

This repository contains a Python implementation of **Graph Cycle Detection** using **Depth-First Search (DFS)**. The program checks for cycles in a directed graph represented as an **adjacency matrix**.

## 📌 How It Works
The code performs DFS traversal and uses a **recursion stack** to detect cycles efficiently.

### 🔥 Step-by-Step Execution

1. **Graph Representation** 📊
   - The graph is represented using an **adjacency matrix**, where `1` indicates an edge between two nodes, and `0` indicates no connection.
   
2. **Initialization** ⚙️
   - The `DFS` class is initialized with:
     - `graph` (Adjacency matrix)
     - `source` (Starting node for DFS traversal)
   - It also maintains:
     - `visited_node` (Set of visited nodes)
     - `recursion_stack` (Stack to track recursion path)
     - `cycle_detected` (Boolean flag for cycle detection)

3. **Depth-First Search (DFS) Traversal** 🔄
   - Starts from the **source node**.
   - Visits adjacent nodes recursively.
   - Keeps track of nodes in the **recursion stack**.
   - If it revisits a node that is already in the recursion stack ➝ **Cycle detected!**

4. **Cycle Detection** 🚨
   - If a cycle is found, the program prints **"Cycle detected!"**.
   - Otherwise, it prints **"No cycle detected."**

## 💻 Example Input & Output
### Input:
```python
source = 2
```
### Output:
```
Graph Adjacency Matrix:
[0, 1, 1, 0, 0, 0]
[0, 0, 1, 1, 0, 0]
[0, 0, 0, 1, 0, 0]
[0, 0, 0, 0, 1, 0]
[1, 1, 0, 0, 0, 1]
[0, 0, 0, 0, 0, 0]
Source node is: 2
DFS Traverse: 2 3 4 1 
Cycle detected!
```

## 📂 Files
- `dfs_cycle_detection.py` → Python script implementing DFS for cycle detection.
- `README.md` → This file (Project documentation).

## 🛠️ How to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/armanHossain4047/Graph-DFS-Cycle-Detection.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Graph-DFS-Cycle-Detection
   ```
3. Run the script:
   ```sh
   python dfs_cycle_detection.py
   ```

## 🤝 Contributing
Feel free to fork this repository, submit issues, or suggest improvements!

## 📜 License
This project is **open-source** and available under the **MIT License**.

Happy Coding! 🚀🎯
