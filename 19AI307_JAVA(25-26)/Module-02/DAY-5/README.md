# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:

Create a class College with a final variable universityName = "Saveetha University". Create objects and print the name.
## AIM:

To write a Java program that demonstrates the use of the final keyword in declaring constants within a class.
## ALGORITHM :

1. Define a class College with a final variable universityName initialized to "Saveetha University".
2. In the main method of class prog:
   * Create an object obj of class College.
   * Access and print the value of universityName.
3. End the program.


## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
class College {
    final String universityName = "Saveetha University";
}

class prog {
    public static void main(String[] args) {
       College obj = new College();
       System.out.println(obj.universityName);
    }
}
```





## OUTPUT:

![alt text](image.png)

## RESULT:

The program successfully demonstrates that a final variable cannot be modified once initialized.