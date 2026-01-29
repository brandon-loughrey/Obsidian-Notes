#### quick sort 
1. select an element in the array called the pivot. 
2. partition the array so that the small entries are on the left, and the large entries are on the right
3. recursively sort the 2 partitions using quick sort

how to implement this partition?
create an array of the smaller elements and an array of the bigger elements. 
![[Pasted image 20260129172045.png]]
In place partition
![[Pasted image 20260129172324.png]]
take the pivot
set big and small
loop until a[small] > pivot - increasing small by 1 
loop until a[big] < pivot - decreasing big by one
swap a[small] and a[big] using a tmp variable 
small = temp
small = big 
big = tmp

return the index of the pivot , big = small
 worst case complexity of partition is o(n)

quick sort complexity 
best case is that every pivot is the median
ever partition has n/2 elements 
has the same complexity as merge sort O(nlogn)

worst case, every pivot is always the least element in every iteration, second partition contains all elements apart from pivot. 

so has n-1 elements 
in consecutive iterations -( time complexity is O(n^2)

why is quick sort used when worst case is as bad a selection sort?

Quick sort in practice runs quicker - doesn't use more memory - memory is expected 

Average case complexity 
Randomised binary search 
guess a random number anywhere in the interval - not the middle number



