
add items with an associated priority queue - when dequeuing it removes the highest priority items first 

a heap is a ADS with a set of items, each with a key. 

ideas to implement 
unsorted array 
Sorted array 
Linked list

Binary Heaps

Max Heaps - higher number = higher priority

for each node - priority > priority of children

We need a complete binary tree to store a binary heap

Bubble_up complexity is O(logn) for insertion 

![[Pasted image 20260216154330.png]]
 in the case that both children are greater than the parent, swap parent with the largest of the 2 children.
 Bubble down complexity is O(logn) 
 
 



