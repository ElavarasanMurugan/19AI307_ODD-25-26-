# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create an abstract class TaxPayer with method calculateTax(). Create subclasses SalariedPerson and BusinessPerson.

For example:
Input 	Result

1       
50000   5000.00

1
72500   7250.00

## AIM:

To write a Java program that demonstrates the use of abstract classes and method overriding for tax calculation of different types of taxpayers.

## ALGORITHM :

1. Define an abstract class TaxPayer with attributes tax and amount, and an abstract method calculateTax().
2. Create a subclass SalariedPerson that extends TaxPayer.
    * Implement calculateTax() to compute tax as 10% of amount.
3. Create another subclass BusinessPerson that extends TaxPayer.
    * Implement calculateTax() to compute tax as 15% of amount.
4. In the main method:
    * Create a Scanner object to read input.
    * Read an integer type to determine taxpayer type.
    * If type == 1, create a SalariedPerson object, read amount, and call calculateTax().
    * If type == 2, create a BusinessPerson object, read amount, and call calculateTax().
5. End the program.





## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.*;
abstract class TaxPayer{
    double tax;
    double amount;
    abstract void calculateTax();
}
class SalariedPerson extends TaxPayer{
    void calculateTax(){
        tax = amount * 0.1;
        System.out.printf("%.2f",tax);
    }
}
class BusinessPerson extends TaxPayer{
    void calculateTax(){
        tax = amount * 0.15;
        System.out.printf("%.2f",tax);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        int type = input.nextInt();
        if(type == 1){
            SalariedPerson obj = new SalariedPerson();
            obj.amount = input.nextInt();
            obj.calculateTax();
        }
        if(type == 2){
            BusinessPerson obj = new BusinessPerson();
            obj.amount = input.nextInt();
            obj.calculateTax();
        }
    }
}
```





## OUTPUT:

![alt text](image.png)

## RESULT:
The program successfully demonstrates the use of abstract classes and polymorphism in tax calculation.