## Advanced decisions 
#### Using logical AND and OR operators
in java we can have multiple conditions in one if statement
We want to be able to check if multiple conditions are true. 
AND - && checks if 2 conditions are true 
OR || checks if at least one condition is true. 

###### Nested if statements
```java 
public class Health{
	public static void main {String[] args}
	if (){
		if(){
		
		}
	}
}
```

###### And operator
```java 
public class Health{
	public static void main(String[] args){
		if (------- && --------){
			
		}
	}
}
```

###### Or operator
```java 
public class Health{
	if (------ || ------){
	
	}
}
```


#### Making accurate and efficient decisions
###### Range checking 
Range checking is a common way of using if statements .

```java 
public class Charge{

if (charge >= 100){
	damage = 10;
}
else if (charge >= 50){
	damage = 5; 
}
else if (charge >= 10){
	damage = 2;
}
}
```

using only if statements has incorrect logic, giving the wrong damage for some values

nesting if statements with an else is better, however is still inefficient, as it uses multiple if statements, and will give the wrong damage for values < 10

using else if statements is the most efficient and most accurate - order is still important to prevent logic errors. 

###### Using many ifs
``` java 
if {
}
if{
}
if{
}
if{ 
}
...
```

switch statements instead 
```java 
switch(){
	case "a" : -------- break;
	case "b" : -------- break;
	case "c" : -------- break;
	...
}
```

Switch statements are good for calling one method, or doing 1 thing. 

#### Using conditional and NOT operators

###### The Conditional operator
The conditional operator is an abbreviated form of the if statement.  
The format is testExpression ? trueResult : falseResult;
define the expression you want to test before the question mark
we define what the true result is between ? and : 
we define false result between : and ;

```java 
health = (health-damage > 0) ? health - damage : 0; 
```
 ###### The not operator
 we use the not operator to negate the result of a boolean expression. 
 NOT is !
 != is NOT EQUAL TO

```java 
boolean dead = false;
	 if (!dead){
		 --------------
	 }
	if (dead != true){
		-------------
	}
```

#### Operator precedence 
```
!
*/%
+-
<><=>=
== !=
&&
||
?:
=
```

#### Decisions in constructors
```java 
public class Weapon{
	int damage;
	int attackSpeed; 
	
	public Weapon (int damage, int attackSpeed){
		if (damage < 0){
			damage = 0;
		}
		else if (damage > 100){
			damage = 100; 
		}
		else {
		this.damage = damage;
		}
		if (attackSpeed < 0 || attackSpeed >10){
			System.out.println("Incorrect attack speed");
		}
		else {
			this.attackSpeed = attackSpeed;
		}
	}
}
```