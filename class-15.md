# Trees

- The root is the top node in a tree
- Left child is the node positioned to the left of a root or node, and the right is on the right
- An edge is a link between a parent and child node
- A leaf is a childless node
- Height is the number of edges from the root to the bottommost node

### Depth First Traversal

- Pre-order goes root >> left >> right
- In-order goes left >> root >> right
- Post-order goes left >> right >> root
- Trees are most commonly traversed with recursion
- With recursion, you add nodes to the stack until you reach a leaf, and then that node will be called off the stack
- Nodes on each new level are treated as the root
- The basic function has three parts:
  1. Check if the is a root.left, if so call the function from that node
  1. Check if there is a root.right, and if so, call the function from that node
  1. Output the root value
- Whichever order you go in will still go to all the nodes, but in different orders

### Breadth First Traversal

- This goes down one layer at a time
- This uses a queue instead of recursion
- First put the root in the queue, then dequeue, but put the left and right child in the queue
- The do the same thing for the new nodes in the queue
- When a node in the queue does not have children, dequeue it without enqueueing anything new

### Binary Trees

- Each node can only have up to two children, but a binary tree can be of any size
- One strategy for adding nodes is to fill up bottom children from the top down
- The height of a binary tree is calculated as log(n), where n is the number of nodes

### Binary Search Trees

- In a BST, all nodes with a lower value than the root are on the left, and all nodes with a higher value are on the right
- Searches can be done quickly, because all you have to do is compare the number you are looking for with the number in the current root
- The time complexity for this is O(h), where h is the height of the tree
