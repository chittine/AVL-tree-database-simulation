# AVL-tree-database-simulation

# AVL Tree Database Simulation (CSE 331 Project)

This project implements an **AVL Tree** — a self-balancing binary search tree — and uses it as the backbone for a simple **table-based database system**. The implementation supports insertion, removal, balancing (via rotations), and several traversal methods, with a visualizer that outputs the tree as an SVG.

---

## Project Overview

- **AVLTree class:**  
  Handles node insertion, deletion, rotations, balancing, and traversal.

- **Node class:**  
  Represents a single node in the AVL tree, with pointers to parent/children.

- **Table class:**  
  A higher-level abstraction that stores rows of data using an AVL tree, enabling efficient lookups and ordered storage.

- **AVLDatabase class:**  
  Simulates a lightweight database capable of processing basic queries such as:
  - `CREATE`
  - `INSERT`
  - `REMOVE`
  - `SHOW ME` (latest, oldest, everything)

- **Visualization functions:**  
  Generate SVG diagrams to visually represent the AVL tree structure.

---

## Key Concepts Demonstrated

- Self-balancing binary search trees  
- Tree rotations (left and right)  
- Recursive tree traversal (inorder, preorder, postorder, level-order)  
- Basic database-like query parsing  
- Data organization using tree structures  

---

## Example Usage

```python
from solution import AVLDatabase

db = AVLDatabase()
db.query("CREATE, employees, ATTRIBUTES name, role, salary.")
db.query("INSERT INTO, employees, ATTRIBUTES name, role, salary, VALUES Alice, Engineer, 90000; Bob, Analyst, 80000 WITH .")
print(db.query("SHOW ME, employees, LATEST."))
