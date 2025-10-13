#### Classes and Objects
###### Classes

In oop we normally create classes used to run applications, I.E. the main class 

Giving this the same name as the file name lets the compiler know it is the main class and should be executed first. 

Everything is a class
Every object is instantiated from a class 
all objects have an is-a relationship with the class it is instantiated from

##### Creating a class
###### Defining a class

A class definition consists of: An optional access specifier, the keyword class and any legal identifier. 

```java 
public class Weapon{
}
class Weapon{}
```

a public class is accesible from anywhere. 

###### Instance Variables
Any class contains variables or data fields

These variables store information about that class 

I.E. vehicle might have topSpeed and numWheels, variables.

When we instantiate an object, each object gets its own copy of all fields in the class. 

```java 
public class Weapon{
	String name;
	int damage;
	double attackSpeed;
}
```

No other classes can access these by default - Data hiding (Encapsulation)

##### Instance methods
###### Parts of a class 


Classes contain fields and methods. 

Methods can be 
Mutators - set or change fields - (Setters)
Accessors - retrieve values (Getters)
Utility - perform related actions without changing values 

```java 
	public void setDamage ( int dam ) {  
	// check damage range  
	 damage = dam ;  
	}  
 
	public int getDamage () {  
	 return damage ;  
	 }  
 
	public double calcDPS () {  
	return damage / attackSpeed ;   }  
```

###### Static vs non static methods
Nonstatic methods are used with object instantiations
these are called instance methods

both static and Nonstatic methods can be used in a class 
static methods are linked to the class and not the object. 

#### Declaring and using objects
###### Instantiating a new object 
To create an object that is an instance of a class:
	Supply a type and indentifier
	Allocate computer memory using the new keyword 
	which creates a reference to an object 
	We can use this reference to access the methods and attributes of the object. 

```java 
public class Example{
	public static void main(String[] args){
		Weapon sword = new weapon();
		sword.setDamage(100);
	}
}
```

###### Data Hiding (Encapsulation)
Data hiding is an OOP design pillar. 
Data fields should be private and inaccessible from a client application
fields should only be accessed using getter and setter methods. 
Clients should not be able to alter assigned values or set values directly.

#### Classes as data types
###### Abstract data type
An abstract data type is a class that we create. 
Implementation is hidden and accessed through public methods. 
This is a programmer defined type and isn't built into the language. 
Defining a data type we need to consider:
	Its name
	its attributes 
	its methods

#### Constructors 
Construct an object 
java creates a default constructor with no arguments, it is used by calling the new keyword
A constructor must have the same name as the class it constructs. 
They cannot have a return type
Generally, they can accept parameters
These parameters define the starting values for data fields
A defined constructor overloads the default.
Multiple constructors can be defined as long as method signatures are different. - name and parameters. 

```java 
public class Weapon{
	private name;
	public Weapon (String n) { 
		name = n;
	}
	public Weapon (String name, int damage, double attackSpeed){
		this.name = name;
		this.setDamage() = damage; 
		this.setAttackSpeed() = attackSpeed;
	}
}
```

###### The this reference
the this reference is used to represent a data field in the class, makes for nicer code.

#### Using static fields
Nonstatic fields are copied for each instance of the class.
if you create 50 instances you get 50 different variables. 
static fields are shared between all instances
if you create 50 instances you get one variable shared by all. 

#### Using existing classes 
Many problems have already been solved by others which are available in classes.  
these classes are built into packages. 
I.E java.lang is imported into every program you write.

###### The math and util classes
the java.lang.Math class contains constants and methods to perform mathematical functions.
it doesnt need to be imported as its part of java.lang 
examples of these classes include java.util, like the scanner class.
###### Importing classes
To use a package not part of java.lang, we use the import statement
this should be done for at the top of any class we want to use the package

```java 
import java.time

public class LocalDate{
	public static void main(String[] args){
		LocalDate today = LocalDate.now()
		system.out.println("Today is: " + today);
	}
}
```
 
#### Composition and Nested Classes
###### Composition
when one class is a data field of another class. 
This object needs to have its values set up like any other class
In this case there is a has-a relationship between the two classes

```java 
public class Inventory{
	Weapon leftHand;
	Weapon rightHand;	
}
```

###### Nested classes
A class containing another class 
static member classes have access to all static methods of the top level class 
Non static methods of the inner class require an instance and have access to all data and methods of the top level classes 
local classes are local to a block
