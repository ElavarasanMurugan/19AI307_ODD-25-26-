# Ex.No:2(B) METHODS

## QUESTION:

Write a method named displayMessage() that prints "Welcome to Java Methods!". Call this method from the main() method.
## AIM:
To write a Java program that demonstrates the use of a method by displaying a message.

## ALGORITHM :

1. Define a class prog.
2. Inside the class, create a method displayMessage() that prints "Welcome to Java Methods!".
3. In the main method:
    * Create an object obj of class prog.
    * Call the displayMessage() method using the object.
4. End the program.



## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
public class prog{
    void displayMessage(){
        System.out.print("Welcome to Java Methods!");
    }
    public static void main(String[] args){
        prog obj = new prog();
        obj.displayMessage();
    }
}
```





## OUTPUT:

![alt text](image.png)


## RESULT:
The program successfully demonstrates calling a method using an object.