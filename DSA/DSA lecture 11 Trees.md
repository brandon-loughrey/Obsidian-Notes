![[Pasted image 20260212170555.png]]

- 2^(n+1) - 1 amnd
- 2^n
- logn (roughly)
- logn 


#### Quad trees 
Useful for representing and manipulating 2d data
#### Ways to implement lists 
Sibling list
essentially a doubly linkes list between siblings 
each node has a pointer to one of its children - each node has pointers to each of its siblings 
![[Pasted image 20260213121548.png]]

Basic - use a doubly linked list format with a left and right pointer to the left and right child and a value pointer (for binary tree) - 

Array - tree[0] is empty 
tree [1] stores the root 
the children of tree[i] are stored at tree[2i] and tree[2i+1]

![[Pasted image 20260213121443.png]]

index of parent of list[i] is list [i div 2]

We can shift this so that list[0] stores the root, in this case,  the children of the ith node in this case is list[2i+1] and list[2i+2]

the parent of the ith node is list[i-1/2]

#### Tree definitions 
a complete tree is stored in an array efficiently, without wasted memory
every level except possibly the last is completely filled, where all leaves are placed as far to ther left as possible

Full binary tree - every node has 0 or 2 nodes 

Complete full binary tree -  a tree that is complete and full

A perfect binary tree - a tree with the max nodes for its height 


#### Searching a tree

Depth first search - search through a tree recursively following each branch until its leaf, and backtracking is the value isn't found


Time complexity - visits each vertex exactly once, constant time per vertex. 

Space complexity - O(depth) - Size of the stack is linear in terms of the depth of the stack 




