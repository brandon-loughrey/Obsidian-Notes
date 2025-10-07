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