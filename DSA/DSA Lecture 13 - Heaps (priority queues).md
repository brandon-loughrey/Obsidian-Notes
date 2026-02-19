
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

deleting arbitrary node, swap leaf with node you delete
compare leaf value to deleted value
if >, bubble up 
if < bubble down 

both heapify up and heapify down have time complexity of o(nlogn)
as bubble up and bubble down are ran n times, and the complexity of bubble up and bubble down both have complexity O(logn)

but heapify down is better, only 1 case can take worst case - the root, but in bubble up - approx 1/2 of elements take the worst case - the leafs

O(nlogn) is not the tightest upper bound for heapify down

Assume perfect tree - 

size n = 2^h+1 -1

h - logn 

total number of swaps is 2+h+1

2^h x 0 + 2^h-1 x 1 + ...... + 1 x h 

which is O(n)


heapsort is O(nlogn)

heapsort is the most modern sorting algorithm





