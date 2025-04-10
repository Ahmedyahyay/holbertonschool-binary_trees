# holbertonschool-binary_trees

This repository contains C functions for working with binary trees, as part of the Holberton School curriculum.

## Repository Information

* **GitHub Repository:** [holbertonschool-binary_trees](https://github.com/holbertonschool-binary_trees)
* **Project:** Binary Trees

## Mandatory Tasks

### 0. New node
* **File:** `0-binary_tree_node.c`
* **Description:** Writes a function that creates a binary tree node.
* **Prototype:** `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`
    * `parent`: A pointer to the parent node of the node to create.
    * `value`: The value to put in the new node.
* **Return:** A pointer to the new node, or `NULL` on failure.
* **Behavior:** When created, a node does not have any children.

### 1. Insert left
* **File:** `1-binary_tree_insert_left.c`
* **Description:** Writes a function that inserts a node as the left-child of another node.
* **Prototype:** `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`
    * `parent`: A pointer to the node to insert the left-child in.
    * `value`: The value to store in the new node.
* **Return:** A pointer to the created node, or `NULL` on failure or if `parent` is `NULL`.
* **Behavior:** If `parent` already has a left-child, the new node must take its place, and the old left-child must be set as the left-child of the new node.

### 2. Insert right
* **File:** `2-binary_tree_insert_right.c`
* **Description:** Writes a function that inserts a node as the right-child of another node.
* **Prototype:** `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`
    * `parent`: A pointer to the node to insert the right-child in.
    * `value`: The value to store in the new node.
* **Return:** A pointer to the created node, or `NULL` on failure or if `parent` is `NULL`.
* **Behavior:** If `parent` already has a right-child, the new node must take its place, and the old right-child must be set as the right-child of the new node.

### 3. Delete
* **File:** `3-binary_tree_delete.c`
* **Description:** Writes a function that deletes an entire binary tree.
* **Prototype:** `void binary_tree_delete(binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to delete.
* **Behavior:** If `tree` is `NULL`, do nothing.

### 4. Is leaf
* **File:** `4-binary_tree_is_leaf.c`
* **Description:** Writes a function that checks if a node is a leaf.
* **Prototype:** `int binary_tree_is_leaf(const binary_tree_t *node);`
    * `node`: A pointer to the node to check.
* **Return:** `1` if `node` is a leaf, otherwise `0`.
* **Behavior:** If `node` is `NULL`, return `0`.

### 5. Is root
* **File:** `5-binary_tree_is_root.c`
* **Description:** Writes a function that checks if a given node is a root.
* **Prototype:** `int binary_tree_is_root(const binary_tree_t *node);`
    * `node`: A pointer to the node to check.
* **Return:** `1` if `node` is a root, otherwise `0`.
* **Behavior:** If `node` is `NULL`, return `0`.

### 6. Pre-order traversal
* **File:** `6-binary_tree_preorder.c`
* **Description:** Writes a function that goes through a binary tree using pre-order traversal.
* **Prototype:** `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`
    * `tree`: A pointer to the root node of the tree to traverse.
    * `func`: A pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
* **Behavior:** If `tree` or `func` is `NULL`, do nothing.

### 7. In-order traversal
* **File:** `7-binary_tree_inorder.c`
* **Description:** Writes a function that goes through a binary tree using in-order traversal.
* **Prototype:** `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`
    * `tree`: A pointer to the root node of the tree to traverse.
    * `func`: A pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
* **Behavior:** If `tree` or `func` is `NULL`, do nothing.

### 8. Post-order traversal
* **File:** `8-binary_tree_postorder.c`
* **Description:** Writes a function that goes through a binary tree using post-order traversal.
* **Prototype:** `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`
    * `tree`: A pointer to the root node of the tree to traverse.
    * `func`: A pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
* **Behavior:** If `tree` or `func` is `NULL`, do nothing.

### 9. Height
* **File:** `9-binary_tree_height.c`
* **Description:** Writes a function that measures the height of a binary tree.
* **Prototype:** `size_t binary_tree_height(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to measure the height.
* **Return:** The height of the tree. If `tree` is `NULL`, return `0`.
* **Note:** Height is defined as the number of edges on the longest path from the root node to a leaf node.

### 10. Depth
* **File:** `10-binary_tree_depth.c`
* **Description:** Writes a function that measures the depth of a node in a binary tree.
* **Prototype:** `size_t binary_tree_depth(const binary_tree_t *tree);`
    * `tree`: A pointer to the node to measure the depth.
* **Return:** The depth of the node. If `tree` is `NULL`, return `0`.
* **Note:** Depth is defined as the number of edges along the path from the root node down to the given node.

### 11. Size
* **File:** `11-binary_tree_size.c`
* **Description:** Writes a function that measures the size of a binary tree.
* **Prototype:** `size_t binary_tree_size(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to measure the size.
* **Return:** The number of nodes in the tree. If `tree` is `NULL`, return `0`.

### 12. Leaves
* **File:** `12-binary_tree_leaves.c`
* **Description:** Writes a function that counts the leaves in a binary tree.
* **Prototype:** `size_t binary_tree_leaves(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to count the number of leaves.
* **Return:** The number of leaves in the tree. If `tree` is `NULL`, return `0`.
* **Note:** A `NULL` pointer is not a leaf.

### 13. Nodes
* **File:** `13-binary_tree_nodes.c`
* **Description:** Writes a function that counts the nodes with at least 1 child in a binary tree.
* **Prototype:** `size_t binary_tree_nodes(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to count the number of nodes.
* **Return:** The number of nodes with at least 1 child. If `tree` is `NULL`, return `0`.
* **Note:** A `NULL` pointer is not a node.

### 14. Balance factor
* **File:** `14-binary_tree_balance.c`
* **Description:** Writes a function that measures the balance factor of a binary tree.
* **Prototype:** `int binary_tree_balance(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to measure the balance factor.
* **Return:** The balance factor of the tree. If `tree` is `NULL`, return `0`.
* **Note:** Balance factor of a node is the difference between the height of its left subtree and the height of its right subtree.

### 15. Is full
* **File:** `15-binary_tree_is_full.c`
* **Description:** Writes a function that checks if a binary tree is full.
* **Prototype:** `int binary_tree_is_full(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to check.
* **Return:** `1` if the tree is full, otherwise `0`.
* **Behavior:** If `tree` is `NULL`, your function must return `0`.
* **Note:** A full binary tree is a tree in which every node other than the leaves has two children.

### 16. Is perfect
* **File:** `16-binary_tree_is_perfect.c`
* **Description:** Writes a function that checks if a binary tree is perfect.
* **Prototype:** `int binary_tree_is_perfect(const binary_tree_t *tree);`
    * `tree`: A pointer to the root node of the tree to check.
* **Return:** `1` if the tree is perfect, otherwise `0`.
* **Behavior:** If `tree` is `NULL`, your function must return `0`.
* **Note:** A perfect binary tree is a full binary tree in which all leaves are at the same depth, and in which every non-leaf node has exactly two children.

### 17. Sibling
* **File:** `17-binary_tree_sibling.c`
* **Description:** Writes a function that finds the sibling of a node.
* **Prototype:** `binary_tree_t *binary_tree_sibling(binary_tree_t *node);`
    * `node`: A pointer to the node to find the sibling.
* **Return:** A pointer to the sibling node.
* **Behavior:** If `node` is `NULL` or the parent is `NULL`, return `NULL`. If `node` has no sibling, return `NULL`.

### 18. Uncle
* **File:** `18-binary_tree_uncle.c`
* **Description:** Writes a function that finds the uncle of a node.
* **Prototype:** `binary_tree_t *binary_tree_uncle(binary_tree_t *node);`
    * `node`: A pointer to the node to find the uncle.
* **Return:** A pointer to the uncle node.
* **Behavior:** If `node` is `NULL`, return `NULL`. If `node` has no uncle, return `NULL`.
