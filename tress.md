# Tress

- Node - A **Tree node** is a component which may contain its **own values**, and references to **other nodes**

- Root - The root is the **node** at the **beginning** of the tree

- K - A **number** that specifies the **maximum** number of **children** any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to **one child node**, in a binary tree
- Right - A reference to the **other child node**, in a binary tree
- Edge - The edge in a tree is the **link** between a **parent** and **child node**
- Leaf - A leaf is a **node** that does **not have** any **children**
- Height - The height of a tree is the number of **edges** from the **root** to the furthest leaf

## Traversals

**Depth First**: 
- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

**Breadth First**: Breadth first traversal **iterates ** through the tree by going through each level of the tree node-by-node. 

**Binary Tree Vs K-ary Trees**: There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows. If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree.

