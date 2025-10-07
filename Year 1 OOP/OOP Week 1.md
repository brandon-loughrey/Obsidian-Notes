In the lab, we used basic methods to take inputs and outputs in the console, and looked at compilation. 

##### Setting up a class, compiling and running code
Before writing any code in java, the class needs to be set up. The file name should have the same name as the Class name. Java is case sensitive, so ensure the case is the same. The class identidfier should start with a capital letter, and every new word should start with a capital letter. 

```java 
public class Example{
	public static void main(String[] args){
	
	}
}
```

In this example the File name Should be Example.java. 

Java code should be compiled and ran in the terminal. 
```
vlab $ javac FileName.java
vlab $ java FileName
```
In the vlab terminal, it should look like this, using javac to compile and java to run.
If there are any syntax errors in the code then it will not compile and an error message will occur. The FileName.class file will not be made.
All lines of code used should end in a ; unless it is a method, which should use {} to open and close.

#### Outputting to the terminal 
To output to the terminal, you use the system command. 
```java
public class Hello{
	public static void main(String[] args){
		System.out.println("Hello World");
	}
}
```
when this code gets compiled and ran, it will output "Hello World" in the terminal. This command should always be used when creating an output to the terminal. 

#### Taking an input from the terminal
To take an input from the terminal you need to use the Scanner library and make a new scanner. 
###### Taking text as an input

``` java 
import java.util.Scanner;

public class Input{
	public static void main(String[] args){
	
	Scanner input = new Scanner(System.in);
	
	System.out.println("Enter your name"); 
	String first = input.nextLine();
	
	System.out.println(first); 
	
	}
	
}
```

using the .nextLine() method reads the text inputted on the next line. In this example, the input is stored to a variable with the identifier first, which id of the type string. 

to concatenate a string you would use the + operator on 2 strings. 


```java
import java.util.Scanner;

public class Input{
	public static void main(String[] args){
	
	Scanner input = new Scanner(System.in);
	
	System.out.println("Enter your first name"); 
	String first = input.nextLine();
	
	System.out.println("Enter your last name"); 
	String last = input.nextLine();
	
	System.out.println(first + "" + last); 
	
	}
	
}
```
This code would output the entered names into the terminal. I.E Brandon Loughrey. 

###### Taking integers as an input

when taking an integer as a function, use the nextInt() method. 
``` java 
import java.util.Scanner

public class age{
	public static void main(String[] args){
		Scanner input = new Scanner(System.in);
		
		System.out.println("Enter your age");
		int age = input.nextInt();
		input.nextLine();
		
		System.out.println("you are " + age + " years old");
	}
}
```

When using the nextInt() method, it is important that it is followed by the nextLine() method to get the end of the line, to ensure that the remaining code can be ran. 

#### Parsing
When changing the data type of a piece of data you need to parse the data,  this is done using the DataType.ParseDatatype method. 

```java 
public class Parsing{
	public static void main(String[] args){
		String number = "1234"; 
		
		int numberInt = Integer.parseInt(number); 
		double numberDouble = Double.parseDouble(number);
		
		System.out.println(numberInt);
		System.out.println(numberDouble);
	}
}
```

In this example, the integer parsed version printed is 1234, and the double parsed version printed is 1234.0. 

#### Operations
In java you can do arithmetic operations, add, subtract , multiply, quotient, modulo.
``` java 
public class Arithmetic{
	public static void main (String[] args){
		int a = 10;
		int b = 3;
		
		// addition 
		System.out.println(a + b);
		
		// subtraction
		System.out.println(a - b);
		
		// multiplication
		System.out.println(a * b);
		
		// quotient
		System.out.println(a / b);
		
		// modulo
		System.out.println(a % b);		

		
	}
}
```

addition, subtraction and multiplication work as expected. 

Quotient truncates the value when integers are used. 

modulo outputs the remainder of the division

#### Working with time

