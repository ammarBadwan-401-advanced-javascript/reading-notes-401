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

* Process continues until you reach a leaf node, where it finds both root.left and root.right to be null, the leaf node will be popped out of the stack and then check for right, repeat until there is nothing left.


### Breadth First

* Breadth traversal uses a queue instead of a stack via recursion.

* First, we enqueue the root, then dequeue it and find its left and its right, then dequeue b and enqueue its right and left, then go to the other in line of stack and enqueue it and then dequeue them all.



### Binary Trees

* Binary restricts the number of children to two, hence the left and right.

* To add a node, we can fill all child spots from the top down by using breadth first traversal.

* Big O time is O(n) because the worst situation is searching the entire tree, Big O of space is O(w) where w is the largest width of the tree.

### Binary Search Trees

* It's a type of tree that does have some structure attached to it, as the nodes are organized in a manner where all values that are smaller than te root are placed left, while bigger are placed on the right

* You can search for the BST easily because you can compare numbers of them, if they are higher than the root number go right, if they are smaller go left.

* Big O of time is o(h) where h is the height, while of space is O(1) because we are not allocating any additional space.

