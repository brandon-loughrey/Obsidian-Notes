memory address into ram , content out of ram

data is stored, managed and manipulated in computer memory
hardware and os work together to allow each running program to see an illusion that they have all the memory of the computer to themselves 
organised as a long list of memory cells, each 1 byte - 8 bits. bits hold either 0 or 1 

you can have explicit memory management with allocate and free  or implicit memory management 

implicit memory management - the programming language itself provides mechanisms to allocate data structures, and identify allocated structures that can no longer be accessed by the running program. 

explicit memory managenment



see slides for how arrays are stored 





Linked lists 
![[Pasted image 20260205173030.png]]


each node contains a value and a memory address


each node takes 8 bytes of memory
4 bytes for data - 4 bytes for memory address


![[Pasted image 20260205174720.png]]
lookup in a linked list - takes O(n) time complexity


Comparison - see slides

![[Pasted image 20260206121141.png]]

Doubly linked lists
store a pointer to the end of the linked list, have backwards pointers too. 

circular linked lists
doubly
make the last node point to the first
make the first node point to the last

singly 
make the last node point to the first
![[Pasted image 20260206122204.png]]

More comparisons
![[Pasted image 20260206122330.png]]

