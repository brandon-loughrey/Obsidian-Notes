#### Sorting
given a set of objects, we can sort on many criteria 
decreasing
alphabetical
increasing most sorting algorithms work on comparisons 
some special cases can be solved without comparisons

all algorithms so far are comparison based 
x < y or x = y or x > y
A slides with waffle about java implementation

#### Bubble Sort
Bubble sort - run through the array and compare every 2 elements, swap elements if in the wrong order. 
Repeat until no swaps made
Worst case complexity in O(n^2)

#### Selection sort
Selection sort
Look through array - find max / min
put to end/ start
repeat for next max/min
worst case is o(n^2)


We want to do better than O(n^2) complexity

#### Divide and conquer (Merge sort)
Divide and conquer is a strategy to reduce one big problem into multiple smaller problems 
Merge sort-
split the array into 2 recursively into smaller problems until you get to individual values
combine back together in order until the full array is smaller

how to merge 2 sorted arrays
allocate a temp array for the result 
if a[i] <= b[j] copy a to temp[i+j]

 complexity is O(nlogn)









