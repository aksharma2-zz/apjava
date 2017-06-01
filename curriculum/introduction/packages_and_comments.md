## What is Java

### Introduction and Java Packages

JAVA was developed by Sun Microsystems Inc in 1991, later acquired by Oracle Corporation. Java is a simple platform independent programming language which is used to create modular and resuable programs. When Java code is compiled(understood by the computer), it is converted into byte code(machine language) which means it can be used across any Operating System like Windows, MAC OS, Linux, etc.

Everything in Java uses Classes and Objects which makes up the building block of Objected Oriented Programming. We will cover about this topic in more detail as you progress through the course. For now, just think of a class as a concept and an object as instance/example of the concept. For eg. class - Car , object - Hyundai. Similarly, class - Animal, objects - Lion, Giraffe, Monkey, etc. For modularity purpose, we group similar classes into a common folder which is known as a package. A good example would be the inbuilt math package provided in Java. The math package provides us with classes which have different mathematical operations like for addition, subtraction, modulus remainder, etc. This is how its used

```
import java.lang.Math;

System.out.print(Math.sqrt(25));
```

By importing the Math package, the programmer can use the inbuilt functions and operations defined by those packages. In this case, the programmer can directly find the square root of 25 by using Math.sqrt instead of making his own functions. 

#### NOTE
	This example is just for demo purposes. The actual code for printing will be defined within a method(which we will discuss later)








