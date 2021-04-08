# Reading 15 Notes

[Home](README.md)

# Trees

## Trees
### Common Terminology
1. Node - A Tree node is a component that may contain it's own values as well as reference to other nodes
2. Root - Root is the node that is the beginning or center of the tree
3. K - This is a number that defines a specific maximum number of children any node may have in a k-ary tree. A binary tree, k = 2
4. Left - Reference to one child node in a binary tree
5. Right - Reference to the other child node in a binary tree
6. Edge - Link between a parent and child node
7. Leaf - A node that does not have any children
8. Height - Number of edges from the root to the furthest leaf

### Binary Tree Vs K-ary Trees
- Binary trees restrict the number of children to two. (left and right children)
- K-ary Trees are if nodes are able to have more than 2 child nodes. In this tree we use k to refer to the max number of children that each node can have. 


### Binary search tree
This is where the nodes are organized where all values that are smaller than the root are placed to the left. And all values that are larger than the root are placed to the right. Searching a BST can be done pretty quickly. All you have to do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller you will only traverse the left side. If the value is larger you only traverse the right. 