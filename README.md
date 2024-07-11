# Difference-Objects-Classes
Difference-Objects-Classes for wk 1 
# Difference-Objects-Classes

This project demonstrates the differences between objects and classes in Java.

## Classes

A class is a blueprint or template that defines attributes and methods that objects created from the class will have. In this project, the `Car` class defines the attributes (make, model, year) and methods (getCarDetails).

## Objects

Objects are instances of a class. In this project, `car1` and `car2` are objects of the `Car` class, each with specific make, model, and year values.

## Code Example

```java
public class Main {
    public static void main(String[] args) {
        Car car1 = new Car("Toyota", "Camry", 2020);
        Car car2 = new Car("Honda", "Civic", 2021);

        System.out.println(car1.getCarDetails());
        System.out.println(car2.getCarDetails());
    }
}

public class Car {
    private String make;
    private String model;
    private int year;

    public Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    public String getCarDetails() {
        return year + " " + make + " " + model;
    }
}
