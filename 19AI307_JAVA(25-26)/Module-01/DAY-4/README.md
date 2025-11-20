# Ex.No:1(D) ARRAYS

## QUESTION:

Write a Java Program to count Even and Odd Numbers in an Array.

## AIM:

To write a Java program that reads an array of integers and counts the number of even and odd elements.

## ALGORITHM :
1. Start the program.
2. Create a Scanner object to read input from the user.
3. Read the size of the array (size).
4. Declare an integer array arr of length size.
5. Initialize counters even = 0 and odd = 0.
6. Loop from i = 0 to size - 1:
    * Read each element into arr[i].
    * If arr[i] % 2 == 0, increment even.
    * Else, increment odd.
7. After the loop, print the number of even elements.
8. Print the number of odd elements.
9. End the program.




## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.Scanner;
public class Average{
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        int size = input.nextInt();
        int[] arr = new int[size];
        int even = 0,odd = 0;
        for(int i=0;i<size;i++){
            arr[i] = input.nextInt();
            if(arr[i]%2==0) even++;
            else odd++;
        }
        System.out.println("Number of even elements: "+even);
        System.out.print("Number of odd elements: "+odd);
    }
}
```





## OUTPUT:

![alt text](image.png)

## RESULT:

The program successfully counts and displays the number of even and odd elements in the array.