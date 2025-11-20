# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:

Write a Java program to calculate the power of a given number.

## AIM:

To write a Java program that calculates the power of a number using Math.pow().

## ALGORITHM :

1. Start the program.
2. Create a Scanner object to read input from the user.
3. Read the base value as a double.
3. Read the exponent value as a double.
4. Use the Math.pow(base, exponent) function to calculate the result.
5. Print the output in the format: 
    * "base raised to the power of exponent is: result".
6. End the program.


## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;
public class PowerCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double base = sc.nextDouble();      
        double exponent = sc.nextDouble();  
        
        double result = Math.pow(base, exponent);  
        System.out.println(base + " raised to the power of " + exponent + " is: " + result);
    }
}

```





## OUTPUT:

![alt text](image.png)

## RESULT:

The program successfully calculates and displays the power of a number.