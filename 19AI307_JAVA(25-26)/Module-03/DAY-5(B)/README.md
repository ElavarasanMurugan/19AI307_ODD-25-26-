# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Find the largest digit in a number using wrapper class methods.

## AIM:


## ALGORITHM :

1. Start the program.
2. Create a Scanner object to read input from the user.
3. Read the input as a string.
4. Convert the string to an integer using Integer.parseInt() (wrapper class).
5. Initialize maxDigit = 0.
6. Repeat while number > 0:
    * Extract the last digit using number % 10.
    * If the digit is greater than maxDigit, update maxDigit.
    * Remove the last digit using number / 10.
7. Print the largest digit.
8. If the input is not a valid integer, catch NumberFormatException and display an error message.
9. End the program.


## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;

public class LargestDigitFinder {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();
        try {
            int number = Integer.parseInt(input);  // Using wrapper class
            int maxDigit = 0;

            while (number > 0) {
                int digit = number % 10;
                if (digit > maxDigit) {
                    maxDigit = digit;
                }
                number /= 10;
            }
            System.out.println("The largest digit is: " + maxDigit);
        } catch (NumberFormatException e) {
            System.out.println("Invalid input. Please enter a valid integer.");
        }
        scanner.close();
    }
}

```





## OUTPUT:
![alt text](image.png)


## RESULT:

The program successfully finds and displays the largest digit in the entered integer.

