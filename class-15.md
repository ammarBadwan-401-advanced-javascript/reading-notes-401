# Trees

## Common Terminology

* Root: its the first or top node in the tree.

* Left child: the node to the left of the root or node.

* Right child: node to the right of a root or node.

* Edge: its the link between a parent and a child node.

* Leaf: leafe is a node that got no children.

* Height: The height of the tree is deteremined by number of edges from root to bottom node.

## Traversal

* You can search the tree by two categories: Depth First and Breadth First.

### Depth First

* Here we prioritize going through the depth (height) of a tree, here are three methods for depth first traversal:

* 1- Pre-Order `root >> left >> right` 2- In-order `left >> root >> right` 3- Post-order `left >> right >> root`.

* Most common way to traverse a tree is **recursion**.

#### Pre-Order

* Pre order means that the root is looked at first, looking means output its value.
first line of code reads this `root.value`,  then the next block of code tells us to check if the root has a left,if yes then send left node to the preOrder method recursively, which means that the left new node is the new root.




### Breadth First




### Binary Trees

### Binary Search Trees