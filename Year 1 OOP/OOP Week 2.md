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
static methodas are linked to the class and not the object. 

