#### Recursion
A method where the solution depends on solutions to the smaller instances of the same problem

Fractal patterns as an example

Recursion requires an end point
#### Factorials
```java 
public static long factorialIter(number){
	long result = 1;
	for(int i = number ; i > 1; i--){
		result *= i;	
	}
	return result;
}

public static long factorialRec(int number){
	if(number == 1){
		return 1; 
	}
	else{
		return number * factorialRec(number-1);
	}
}


```

when choosing between recursion and iteration, we have to consider the number of method calls - ensure the call stack doesn't get full - gives errors
#### Fibonacci
```java
public long fibonacci(int _index){
	long[] valueArray = new long[_index]
	valueArray[0] = valueArray[1] = 1; 
	for (int i =2 , i < _index; i ++){
		valueArray[i]  = valueArray[i-1] + valueArray[i-2];
	}
	return valueArray[_index - 1];
}
```

#### Iteration vs recursion

###

