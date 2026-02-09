![[Pasted image 20260209150617.png]]

Example use - print queue 

queues need  2 pointers - front and rear 

enqueue and dequeue by moving the pointers 

Queue as array problem 
run out of memory space with dequeues - front = rear = maxsize; 

cannot enqueue any elements 
Solution - Circular queue - move the rear to the front; 

move by 1 position calculated by 

(pos+1) % circle length, circle length = MAX_SIZE
![[Pasted image 20260209154503.png]]

