** Input and Output **

For this course, to accept arbitrary value from user it willbe displayed like

```
double x = IO.readDouble(); // get user input
```

*** Output ***

The two main ways to display output is by **System.out.print()** and **System.out.println()** where the latter adds a new line break after every argument while the former does not. In Java, everything can be printed even null values and errors provided we know how to print them.

	```
	System.out.print("Hello");
	System.out.print("World");  

	// prints Hello World

	System.out.println("Hello");
	System.out.println("World");

	//prints Hello
			 World

	System.out.print( (8 == (4+3)) ) // prints false because 8 <> 7

	int x=3;
	System.out.print("My value is"+x)l // prints My value is 3

	```

*** Special Escape characters ***

	Special characters which have a backslash followed by a single character

	* \n - new line or line break
	* \" - add a double quote to be printed
	* \\ - backslash

```
System.out.print("Hello \n World");
// prints Hello
		  World

System.out print("Here is \" Harry Hacker\" "); // prints Here is "Harry Hacker"
```


