#### Arrays - advanced concepts
##### Arrays and methods
Primitive data types pass to a method by value. 
Arrays and objects are passed into methods by reference 
##### Parallel arrays 
having multiple arrays with the same number of elements. 
the same index/subscript of each array is related to each other. 
e.g. an array of names or an array of marks. 
##### Array sorting
import java.util.Arrays and use the sort methodn to sort. 
sorting to arrange objects

##### 2D arrays
1d array is a standard array
2d array can be thought of as a table - i.e a spreadsheet - rows and columns. 
arrays can be accessed directly
2d arrays use 2 sets of [] to define 
```java 
import java.util.Scanner

public class Triangle{
	public static void main(String[] args){
		String[][] map = new String[size][size];
		final int SIZE = 10; 
		int playerX = 5;
		int playerY = 5;
		Scanner scanner = new Scanner(System.in);
		
		for (int y = 0 ;  y < SIZE ; y++ ){
			for (int x = 0 ; x < SIZE ; x++){
				map[y][x] = '.';
			}
			map[playerY][playerX] = '@';
		}
		for (int y = 0 ;  y < SIZE ; y++ ){
			for (int x = 0 ; x < SIZE ; x++){
				system.out.print(map[y][x]);
			}
			System.out.println();
		}
		while(true){
			String direction = scanner.nextLine();
			
			switch (direction) {
				case "a": playerX--; break;
				case "d": playerX++; break;
				case "w": playerY++; break;
				case "s": playerY--; break;
		
			}
		}
	}
}
```
