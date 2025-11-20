# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
If an Integer object is set to null, and you attempt to call .toString() on it, what happens? How can you prevent your code from throwing an exception in such cases?

## AIM:

To write a Java program that demonstrates how a NullPointerException can occur when working with wrapper classes and how to handle it using a try-catch block.
## ALGORITHM :

1. Start the program.
2. Create a Scanner object to read input from the user.
3. Read an integer input.
4. Assign num as an Integer object:
    * If input == 0, assign null.
    * Otherwise, assign the integer value
5. Use a try block:
    * Attempt to print num.toString().
6. If num is null, a NullPointerException will be thrown.
7. Catch the exception in the catch block and print "Null Integer".
8. Close the scanner.
9. End the program.




## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:


```java
import java.util.Scanner;
public class NullPointerIntegerExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int input = sc.nextInt();
        Integer num = (input == 0) ? null : input;
        try {
            System.out.println(num.toString());
        } catch (NullPointerException e) {
            System.out.println("Null Integer");
        }
        sc.close();
    }
}

```




## OUTPUT:

![alt text](image.png)


## RESULT:

The program successfully demonstrates exception handling for NullPointerException.