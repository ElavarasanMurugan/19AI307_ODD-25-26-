# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to demonstrate the concept of an inner class. The program should contain an outer class with a method and an inner class with another method. Create objects of both classes and display their outputs.

## AIM:

To write a Java program that shows how to declare and use an inner class in Java, and to understand how objects of inner classes are created using an outer class object.
## ALGORITHM :

1. Start the program.
2. Create an Outer class with a method outerMethod() that prints a message.
3. Inside the Outer class, create an Inner class with a method innerMethod() that prints a message.
4. In the main() method:
    * Create an object of the Outer class.
    * Call the outerMethod().
    * Create an object of the Inner class using:
    * Outer.Inner inner = outer.new Inner();
    * Call the innerMethod().
5. Display the output.
6. End the program.



## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:


```java
class Outer {
    
    void outerMethod() {
        System.out.println("This is the Outer class method.");
    }

    // Inner class
    class Inner {
        void innerMethod() {
            System.out.println("This is the Inner class method.");
        }
    }
}

public class InnerClassDemo {
    public static void main(String[] args) {

        Outer outer = new Outer();
        outer.outerMethod();

        Outer.Inner inner = outer.new Inner();
        inner.innerMethod();
    }
}

```




## OUTPUT:

This is the Outer class method.
This is the Inner class method.


## RESULT:

The program successfully demonstrates the use of inner classes.

