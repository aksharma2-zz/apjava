## Access Specifiers

Access Specifiers are used to define access to variables and methods (whether it is free or restricted)
The three main types of access specifiers are

*	Private - variables and private methods can only can only accessed by methods of that class. They belong to the class only.
*	Public - public variables and methods can be accessed from anywhere and by anyone.
* 	Protected - protected methods can be accessed by classes within same package or classes in a different package but inherit the class

For this course, we will cover the first two access specifiers only. Lets consider our previous Employee example

1. All the private instance variables are used directly only by the methods defined for the Employee class. Even objects of class Employee cannot use these private instance variables directly.

2.	All objects of Employee class can access any public method defined by the class. For eg. trump object reference could call setSal method and change its assigned salary to a new salary. If a public instance variable was declared by the class, then the object could directly access and modify the variable. However, this is generally avoided such that an outside client cannot directly change the value of a variable to an arbitrary pre chosen value. He should be allowed to only interact with methods which carry out particular tasks. This concept is known as **Data Encapsulation** which is the process of hiding inner implementation details to the outside world.

3.	*Static variables* are a special type of variable which belong to the class and are shared across all objects of the class. It is called static because it is created only once. Some uses for making static variables are
	
	*	keep track of total number of objects
	*	accumalate a total

For our case, our static variable was companyCommission and is shared across all Employee objects. Static variables are accessible to non static methods. What this means is that all Employee objects can access companyCommission variable as long as they have a public method which can access it. As we can see from implementation of setCommission method, only if an Employee object is a manager, he can change the commission value. Hence, only trump object can change it. However, any object can access the value of companyCommission through the getCommission method.
