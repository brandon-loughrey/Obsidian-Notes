#### Quicksort #
- slow when smallest/biggest item chosen as pivot
- O(nlogn) comparisons in best case 
- O(n^2) in worst case

average case- 

finding the kth smallest element
methods 
sort the array, pick the kth one - nlogn 

quick select - O(n)

follow quick sort
disregard irrelevant sides
n + n/2 = n/4 + ..... = 2n

hence we have o(n) complexity

Heapify - bubble up vs bubble down  

[10,9,8,7,6,5,4] is a sorted array - descending order - max heap 

we want a min heap- we also use heapify down, but change the code for bubble down 

Are all sorts the same?
Merge Sort

Attempting to merge all parts together

select minimum of first element in each array
move min to the next part of first array

create a min heap of the elements 

How to analyse the complexity of an algorithm given in code 

```python 
def f(n):
print(n)
if n <= 1:
return 
else:
f(n//2)


```

complexity is log_2(n)

```python
def fc(n):
print(n)
if n <= 1:
return 
if fc(n%2==0):
	fc(n//2)
else:
   fc(3*n + 1)
```
 Collatz conjecture says 
 fc always terminates 

  Rice's theorem 
  It is undecideable whether a given code runs in time O(n^2)

```java 
int function1(int[] array){
	int n = array.length; 
	for(int i = 0; i <n ; i++){
		function2(array,i,n);
	}
}
```
What is the complexity if function2 takes logn?

give the best upper bound 
we could say
t1(n) <= n x t2(n)
nlogn

Is this the best upper bound?

t1(n) = t2(n) + t2(n-1) + ---- + t2(1)

complexity of t2 is $\sum_{i=1}^{n}\log{i}$

which is O($\log{n}$)

t2 is O($\log{n!}$)
which is $\\theta$(n\log{n})$
or $O(\frac{n}{2}\log{n} - \frac{n}{2})$


think based on lower bound of on sorting the complexity of bubble sort

Merge sort, quick sort, other recursive algorithms 

For merge sort 
t1(n) = t2(n)+2x(t2(n/2))


If you dont know the general expression write small ones and try spot a pattern 

there is logn lots of ns 
complexity is nlogn 

We can do the same thing for other D&C algorithms


```java 
int function1(int[] array){
	int i = array.length;
	while (i > 1){
		function2(array,0,i);
		i/=2 
	}
}
```

naive upper bound - # of iterations x time of 1

case a f2 take O(n)

naive upper bound is O(nlogn)

but we can get upper bound of O(n)
 using sums 
 









