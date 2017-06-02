## Classes and Objects

Classes and Objects is the building block of Java and one of the most important topics. Everything in Java is considered as an Object, a single instance of a particular blueprint, a class. If you remember, the way to create integers was

```
int index = 0;
```

However, the inner working of Java creates an integer in somewhat the following way

```
Integer index = new Integer(0);
```
As we can see from above, our object (index variable) is a new instance of type Integer with instantiated value of 0

A class can be thought of like a blueprint which defines instance variables(variables belonging to a class) and methods which will be implemented by its objects. Different objects can have different values depending by what values they are instantiated with. For eg. lets create an example of an employee blueprint and instantiate different employees. A variable that represents an object is known as object reference

```
class Employee{

	private String name;
	private String EID;
	private double sal;
	private boolean isManager;
	private static int companyCommission = 500; 

	public Employee(){		// Constructor 1 i.e. default constructor
		name = "John Doe";
		EID = "123";
		sal = 1000;
		isManager = false;
	}

	public Employee(String name, String EID, double sal, boolean isManager){	// Constructor 2 i.e. parameterized constructor
		this.name=name;
		this.EID=EID;
		this.sal=sal;
		this.isManager=isManager;
	}

	public double getSal(){	//getter aka accessor method
		return sal;
	}

	public void setSal(double newSal){	//setter aka mutator method
		this.sal = newSal;
	}

	public void setSal(double newSal, int bonus){ // overloaded method
		this.sal = newSal + (newSal * bonus);
	}

	public void setCommission(int newComm){ // setter #2
		if(isManager) // same as writing isManager==true . only if employee object is a manager, he can change commission
			companyCommission = newComm;
	}

	public int getCommission(){	//getter #2
		return companyCommission;
	}

	public static void changeCommission(int newComm){
		companyCommission = newComm;
	}
}

Employee default = new Employee(); // 'default' object reference instantiated with no values hence will take default values from Constructor 1

Employee mike = new Employee("Mike", "456", 20000, false); // 'mike' object reference instantiated with user defined values so Constructor 2 will execute in this case

Employee trump = new Employee("Trump", "999", 100000, true); // 'trump' object reference instantiated with user defined values
mike.setSal(30000); // new Salary for mike
trump.setSal(120000, 0.2); // new Salary for trump along with bonus

trump.setCommission(1000);
System.out.print(mike.getCommission()); // prints 1000;

mike.setCommission(1500);
System.out.print(mike.getCommission()); // prints 1000 (value doesnt change to 1500) . Mike is not a manager so he cannot change commission.

trump.setCommission(2000);
System.out.print(default.getCommission()); // prints 2000;

Employee.changeCommission(3000); // commission is now 3000
```

As we go through the chapter, we will keep this example and discuss it further.













