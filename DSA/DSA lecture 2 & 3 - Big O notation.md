the precise number of steps is too detailed to get a clear understanding. 

difference between n and 2n is insignificant comapared to the the difference between n and n^2 
i.e doing a comparison and a multiplication is 2n
doing a comparison or a multiplication is n 

the solution is to simplify to the headline complexity

complexity in terms of input size

if we know an algorithms time performance and space performance, we dont have a way to look at how this scales with the number of inputs.

number of steps measured up to is a constant factor to have a measure independent of the machine.

we give an upper bound in the form f(n)<= Cg(n) for some constant c > 0; 

ie 4n+3 <= Cn
n^3 + 2n^2 + n + 20 <= Cn^3 

We use the Big O notation

f(n) belongs to O(g(n)) if 
there exists C,n0 > 0 s.t for all n >=n0 |f(n)| <= |Cg9n)|

formally O(G(n)) is a set of functions, that do not grow at a faster rate than g. 

'f does not grow at a quicker rate than g' 

it is often common to write f(n) = O(g(n))

this is an **Abuse of notation**

"3n^2 + 4 = O(n^2)"
is shorthand for 3n^2 + 4 <= cn^2 for all ...

f <= g big o 
f >= g Omega 
f = (approximately) g - theta

how to prove that the reverse case is not true

invert the statement

choose value c and n0 

pick n > c,n0

2^n > cn^2 

cn^2 > n^3 

2^n > n^3 

when n > 16

prove by induction

Assume 2n > n^3

show 2^n+1 > (n+1)^3


