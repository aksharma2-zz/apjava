** Control Structures **

Control Structures are structures in programming languages which are used to make decisions based on user choices and actions. They are categorized mainly into

* Decision making
* Loops

1. Decision making

It is used to evaluate whether a condition matches a certain value and returns a boolean value using which we can carry out actions and decide which path to follow;

	*** THE if STATEMENT ***

		The if statement is executed only if the condition is true otherwise it doesn't carry out the action. For eg.

		```
		int x = 3;
		if(x>=3){
			System.out.print("value of x is"+x);
		}
		System.out.print("\t End program");
		```

		The above program prints : value of x is 3	End program 
		This is because since x is equal to 3, if condition is satisfied and carries out the actio which is enclosed by the parantheses

	*** The if...else STATEMENT ***

		This is an extension of if but in this case we can specify another path which the computer we can take in case our condition was not true. For eg.

		```
		int x=5;
		if(x>10){
			x=20;
		}
		else{
			x=0;
		}
		System.out.print("value of x is +"x); // prints value of x is 0
		```

		*** THE if...elseif...else STATEMENT (EXTENDED if)

		This is also like the previous cases except for this case we can specify multiple checking conditions. For eg.

		```
		int x=7;
		int y;

		if(x>10){
			y=10;
		}

		else if(x<20){
			y=20;
		}

		else{
			y=30;
		}
		System.out.print("value of y is "+y); // prints value of y is 20
		```

	*** The NESTED if statement ***

		If a statement is a part of another if statement embedded inside the latter's parantheses scope then it is known as a nested if statement. For eg.

		```
		int x=5;
		int y;
		if(x>0)
			if(x%2==0)
				y=10;
		else
			y=20;

		System.out.print(y); // prints 20
		```

		Beware of the example given above. It is meant to confuse you. From the indentation, it seems as if else condition is in continuum with the first if condition. However, it is continuum with the second if condition. This is because for just 1 statement after an if condition, it is not neccessary to add parantheses. However, it is a good practice to add proper indentation and parantheses to avoid these mistakes.

		```
		int x=5;
		int y=0;

		if(x>0){
			if(x%5==0){
				y=10;
			}
		} 
		else{
			y=20;
		}

		System.out.print(y); // prints 0 
		```

		Now we can see, it is much more readable and the else condition is now in continuum with the first if condition. Now since the first if condition is satisfied, the else condition is never reached.

2. Loops

As the name sounds, Loops are control structures used to execute repeated actions until the condition is evaluated to be false. The three main types of loops are

* for LOOP
* while LOOP
* for each LOOP (aka enhanced for LOOP)

1. for LOOP
	
	General form is : for(*loop variable initilization*; *termination condition*; *update variable value*){ do something }
	The termination condition is tested at the top of the loop i.e. the first step of the loop. The variable is updated at the end of the loop i.e. the last step of the loop. For eg.

	```
	for(int i=0; i<5; i++){
		System.out.print(i);
	}
	// Prints 01234 . Take note that it does not print 5 because loop terminates as soon i becomes equal to 5 and loop works only if i is less than 5

	for(int index=20; index>=10; index=i-2){
		System.out.print(index+" "); // add extra space after every number printed 
	}
	// Prints 20 18 16 14 12 10

2. while LOOP
	
	The loop works almost the same way like the for loop but except the syntax is different. The general form is while(*boolean test on variable*){	
		do something
		*update variable
	}

	For eg.

	```
	int index=0;
	while(index<5){
		System.out.print(index);
		index++;
	}

	// Prints 01234

3. for each LOOP

	To understand this loop completely, we need to cover the topic of Arrays and Collections. However, think of it is a way that given a collection of items of a similar kind, the loop automatically traverses over the collection one by one till it reaches the end. The advantage of using this loop is the relatively easy syntax but however, it restricts freedom to write code our own way as it follows a particular convention. The general form is (*variable* : *collection*){ do something } For eg.

	```
	int[]collection = {0,1,2,3,4};
	for(int i: collection){
		System.out.print(i);
	}

	// Prints 01234







