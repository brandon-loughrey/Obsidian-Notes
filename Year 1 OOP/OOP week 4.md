#### For loops
Both for and while loops have 3 basic components 
-Initialisation
-checking 
-alteration  
(of the control variable)
```java 
int count = 0; 
while (count<5){
	-----
	count ++
}
```

For loop has all 3 aswell
```java 
for(int i=0 /*initialisation*/ ; i < 5 /*condition*/ ; i++ /*Alteration*/){
	-----
}
```

Components separated by ; as each part is essentially an individual Java Statement

##### For loop variations
more than one value can be initialised for a value in a for loop
check multiple values using && and || operators

We can alter more than 1 value 

```java 
for (int count = 0 , int i = 10, count < 5 , count ++, i--){
	System.out.println("counting down: " + i + "...");
}
```

#### Nested loops
A loop inside another loop
we can combine different kinds of loop
the inner loop must be entirely contained in the outer loop

example- print numbers from 1 to n in ascending order 

```java 
import java.util.Scanner;

public class Nested{
	public static void main(String[] args){
	
		Scanner input = new Scanner(System.in);

		System.out.println("enter a number")
		int n = input.nextInt();
		
		for (int i = 0 ; i < n ; i++){
			for (int j = 0 , j < i + 1 ; j++){
				System.out.print(j+1);
			}
			System.out.println();
		}
	}
}
```

be considerate of scope when using nested loops
#### Loop control statements
can be used to change the behaviour of a loop
break - exits loop entirely
continue - skips the current iteration and continues with the next iteration 

Example - searches for a number in the range (0,100), printing all searched values that are not divisible by 3 

```java 
import java.util.Scanner 
public class Search{
	public static void main(String[] args){
		Scanner in = new Scanner(System.in);
		
		for (int i = 0 ; i < 100 ; i++){
			if (i%3 == 0){
				continue;
			}
			/*if (i%3 == 0) continue;*/
			if (i==n){
				System.out.println(n + " Found!");
				break;
			}
			System.out.println("Doing some complicated calculation with " + i);
		}
	}

}
```

#### Loop performance 
Avoid unnecessary operations - if you can do something outside of the loop then do that

avoid nesting loops - if not required dont nest a loop

Consider what code to put in loops - I.E  calling methods which contains a loop

Especially avoid multiple levels of nested loops- dont go deeper than 3 levels

#### Common mistakes 
Forgetting to alter variable
forgetting to include {} - incomplete loop body
Repeat steps within a loop that could be done outside the loop

