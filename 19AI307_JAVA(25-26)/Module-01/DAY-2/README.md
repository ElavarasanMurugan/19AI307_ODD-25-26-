# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
In a magical building, an elevator behaves oddly:

If the floor number is divisible by 3 and 5, it says "Skipped".

If the floor number is divisible by 3 only, it says "Beware!".

If the floor number is divisible by 5 only, it says "Blessings!".

Otherwise, it announces the floor number - print - "Floor {number}" .

Write a Java program to simulate this elevator logic for a given floor number.

## AIM:

To write a Java program that reads an integer and prints different messages based on divisibility conditions with 3 and 5.

## ALGORITHM :
1. Start the program.
2. Create a Scanner object to read input from the user.
3. Read an integer n from the user.
4. Check conditions in order:
    * If n is divisible by both 3 and 5, print "Skipped".
    * Else if n is divisible by 3, print "Beware!".
    * Else if n is divisible by 5, print "Blessings!".
    * Else, print "Floor n".
5. End the program.



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        int n = input.nextInt();
        if(n%3 == 0 && n%5==0){
            System.out.println("Skipped");
        }
        else if(n%3 == 0){
            System.out.println("Beware!");
        }
        else if(n%5 == 0){
            System.out.println("Blessings!");
        }
        else{
            System.out.println("Floor "+n);
        }
    }
}
```





## OUTPUT:

![alt text](image.png)


## RESULT:

The program successfully checks divisibility and prints the correct message.