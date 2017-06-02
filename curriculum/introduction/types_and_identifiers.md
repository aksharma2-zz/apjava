## Types and Identifiers

### Identifier

An identifier is the name for which identifies a entity in Java (i.e. a variable, parameter, constant, method or even a class). The rules for an identifier are

	*	It cannot begin with a digit
	*	It is case sensitive (number is not the same as Number)
	*	It cannot be the same as a predefined keyword (for eg. cannot be int, this, boolean, etc.)

There are different data types of variables which Java allows us to declare which are
	
	1.	int - Whole number integers . For eg. -2, 5,1000
	2.	double - Decimals . For eg. -2.44, 455.124
	3.	boolean - True or False value . true or false only
	4.	float - Floating point value with lesser range than double . For eg., 1.5f, -444.2f (Not to be covered)
	5.	void - empty return type which doesn't return anything. For eg., adding two numbers but not displaying or using the final value


###	 Type Casting

Type Casting is a feature used by Java which allows the compiler to change the data type of variables from one form into another. For eg., to type cast a double value into an int value. The code and their outputs are

```
int a;
double x,y,z,avg;
boolean val;

a= 10;
x= 3.6
y=5.6;
z=3;   // z will be assigned value of 3.00 as it is type double

avg = (x+y)/2;   // value of avg -> 4.6
avg = (int)avg;  // value of avg -> 4
val = false; // will display false
a = (int)val // will have value 0 because in Java when you typecast boolean to int, false ->0 && true->1


