## [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

![slk](https://miro.medium.com/max/975/1*PWJiwTxRdQy8A_Y0hAv5Eg.png)
**Trees**
  * Terminology
    - Node - A Tree node is a component which may contain it’s own values, and references to other nodes
    - Root - The root is the node at the beginning of the tree
    - K - A number that specifies the maximum number of children any node may have in a k-ary tree.
    - Left - A reference to one child node, in a binary tree
    - Right - A reference to the other child node, in a binary tree
    - Edge - The edge in a tree is the link between a parent and child node
    - Leaf - A leaf is a node that does not have any children
    - Height - The height of a tree is the number of edges from the root to the furthest leaf.
  * Traversals - traversing a tree allows us to search for a node, and print out the contents of a tree
    - 2 categories of traversals:
      * Depth First - prioritizes going through the depth of the tree first and there are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. To traverse through a tree is to use recursion. 
        - 3 methods of Depth First: 
        Pre-order: root >> left >> right
        In-order: left >> root >> right
        Post-order: left >> right >> root
      * Breadth First - iterates through the tree by going through each level of the tree node-by-node
  * Binary Tree Vs K-ary Trees
    - Binary Trees - restrict the number of children to two, no specific sorting order, and nodes can be added into a binary tree wherever space allows
    - K-ary Trees - nodes that are able to have more than two children. K refers to the maximum number of children that each Node is able to have
      * Breadth First Traversal - requires a similar approach to the breadth first traversal by still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child.
      * Adding a node - is to fill all “child” spots from the top down, and to do so leverage the use of breadth first traversal. If you want to add a a node placed in a specific location, you need to reference both the new node to create, and the parent node upon which the child is attached to.
      * Big O time complexity for inserting a new node is O(n).
  * Binary Search Tree (BST) - a type of tree that does have some structure attached to it, and nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.
    - Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h).
