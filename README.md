# JAVA CLASS WITH CONSTRUCTORS

package com.sharon;

public class car {
	String brand ;
	String model ;
	int year;
	
	public car() {
		this.brand= "Unknown";
		this.model= "Generic Model";
		this.year= 2026;
		System.out.println("Default Constructor called : created a generic car.");
		
	} 
	
	
	public car(String brand , String model, int year) {
		this.brand = brand;
		this.model=model;
		this.year=year;
		System.out.println("Parameterized Constructor called : Created a " + brand +" "+ model + " .");
	}
	
	public void displayDetails() {
		System.out.println("Car Details -> Brand: "+brand+" | Model: "+model+" | year: "+year);
	}
}

# CLASS IMPLEMENT

package com.sharon;

public class Main1 {

	public static void main(String[] args) {
		System.out.println("Displaying Objects and Contructors in Java");
		
		car defaultCar = new car();
		defaultCar.displayDetails();
		
		car Car1 = new car("Toyota","Camry",2024);
		Car1.displayDetails();
		
		car Car2 = new car("Tesla","Model 3",2025);
		Car2.displayDetails();
	}
}
# OUTPUT

Displaying Objects and Contructors in Java

Default Constructor called : created a generic car.

Car Details -> Brand: Unknown | Model: Generic Model | year: 2026

Parameterized Constructor called : Created a Toyota Camry .

Car Details -> Brand: Toyota | Model: Camry | year: 2024

Parameterized Constructor called : Created a Tesla Model 3 .

Car Details -> Brand: Tesla | Model: Model 3 | year: 2025

