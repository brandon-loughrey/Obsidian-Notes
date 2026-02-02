- A type is a set of possible values 
- with a set of allowed operations on those values
an abstract data type is one whose internal representation is hidden to the user
Users of an abstract data type may have no information about how it is implemented 
depends only on the published information about how it behaves

#### Lists 
a list is an ordered collection of elements. 
operations may include 
insert 
delete 
get length 
access data by position
concatenation
searching 
sorting 

different implementations of lists 
Arrays
Linked Lists 
others 

A list is an ADT 
there are different implementations of a list in java 
I.e. arraylist, LinkedList 

Arrays as lists 
The basic array data type has a few operations 
...

What doesnt it have
- Inserting

Dynamic arrays 
start with 128 entries in an array
let n = 128+128k for some k 
128 insertions 
128 copies + 128 insertions
256 copies + 128 i 
...

complexity is o(n^2) (see pf in slides)

amortized complexity - cost of 1 insertion 

= O(n)

see pf in slides 


#### Better approach
initially allocate 128 entries 
whenever becomes full - double size

i.e 
128 i 
128c + 128i
256c+256i
512c + 512i 

complexity is o(n) see pf in slides 

amortized complexity o(1) see pf in notes



