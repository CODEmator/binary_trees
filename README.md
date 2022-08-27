**Binary Tree**
A binary tree is a tree data structure in which each node has at most two children, which are referred to as the left child and the right child. A recursive definition using just set theory notions is that a (non-empty) binary tree is a tuple (L, S, R), where L and R are binary trees or the empty set and S is a singleton set containing the root. Some authors allow the binary tree to be the empty set as well.
**Data structures**

Please use the following data structures and types for binary trees. Don’t forget to include them in your header file.

**Basic Binary Tree**

```
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
```

**Binary Search Tree**

```
typedef struct binary_tree_s bst_t;
```

**AVL Tree**

```
typedef struct binary_tree_s avl_t;
```

**Max Binary Heap**

```
typedef struct binary_tree_s heap_t;
```

**Note:** For tasks 0 to 23 (included), you have to deal with simple binary trees. They are not BSTs, thus they don’t follow any kind of rule.
**Print function**
To match the examples in the tasks, you are given this function
```

                           .----------------------(006)-------.
                      .--(001)-------.                   .--(008)--.
                 .--(-02)       .--(003)-------.       (007)     (009)
       .-------(-06)          (002)       .--(005)
  .--(-08)--.                           (004)
(-09)     (-07)

```
This function is used only for visualization purposes. You don’t have to push it to your repo. It may not be used during the correction

