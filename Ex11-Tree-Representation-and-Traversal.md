# Ex11 Tree Representation and Traversal
## DATE:
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start
2.Define a function display_postorder() that takes a pointer to the root node of the tree. 
3. Check if the current node (root_node) is not null.
4. Recursively call display_postorder() for the left child of the current node. 
5. Recursively call display_postorder() for the right child of the current node.
6. After visiting both children, print the value of the current node.
7. End  

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: GANESH PRABHU J
RegisterNumber: 212223220023
*/

struct node
{
int value;
struct node*left_child, *right_child;
};*/
void display_postorder(struct node*root_node){ if(root_node)
{
display_postorder(root_node->left_child); display_postorder(root_node->right_child); printf("%d\n",root_node->value);
}
}
```

## Output:

<img width="723" height="405" alt="437354782-34f755c6-270d-40a2-9653-aad65d2e2b35" src="https://github.com/user-attachments/assets/8e2e9340-c31e-4bee-aa6c-83d497a5ff11" />


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
