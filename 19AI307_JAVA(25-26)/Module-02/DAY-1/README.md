# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:

Create a class Car with attributes brand, model, year. Create 2 objects and print their details.
## AIM:

To write a Java program that demonstrates the use of a class by creating objects and displaying their attributes.

## ALGORITHM :

1. Define a class Car with three attributes: brand, model, and year.
2. In the main method, create the first object car1 of class Car.
    * Assign values to its attributes (Toyota, Innova, 2022).
3. Create the second object car2 of class Car.
    * Assign values to its attributes (Hyundai, i20, 2021).
4. Print the details of both cars using System.out.println().
5. End the program.




## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:


```java
class Car{
    String brand;
    String model;
    int year;
}
public class prog {
    public static void main(String[] args) {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}

```




## OUTPUT:

![alt text](image.png)

## RESULT:

The program successfully creates two car objects and displays their details.