# Ex.No:3(D)    INTERFACE 

## QUESTION:

You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.

Bot Types:

SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".

RainBot: Predicts "COLD" if temperature < 20, else "WARM".

Input:

temperature

botType (1 for SunBot, 2 for RainBot)Output:

Prediction as a string.
## AIM:

To write a Java program that demonstrates the use of interfaces and polymorphism by predicting weather conditions using different bots.

## ALGORITHM :

1. Define an interface Bot with a method predict(int temp) that returns a String.
2. Create a class SunBot that implements Bot.
    * In predict(), return "HOT" if temp > 30, otherwise return "MODERATE"
3. Create another class RainBot that implements Bot.
    * In predict(), return "COLD" if temp < 20, otherwise return "WARM".
4. In the main method:
    * Create a Scanner object to read input.
    * Read temperature (temp) and type (type).
    * If type == 1, create a SunBot object.
    * Else, create a RainBot object.
    * Call predict(temp) using the chosen bot object.
    * Print the prediction.
5. End the program.





## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:


```java
import java.util.*;
interface Bot{
    public String predict(int temp);
}
class SunBot implements Bot{
    public String predict(int temp){
        return (temp>30) ? "HOT" : "MODERATE";
    }
}
class RainBot implements Bot{
    public String predict(int temp){
        return (temp<20) ? "COLD" : "WARM";
    }
}
public class Main{
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        int temp = input.nextInt();
        int type = input.nextInt();
        
        Bot obj;
        if(type == 1){
            obj = new SunBot();
        }
        else{
            obj = new RainBot();
        }
        System.out.println(obj.predict(temp));
    }
}
```




## OUTPUT:

![alt text](image.png)

## RESULT:
The program successfully demonstrates the use of interfaces and polymorphism to predict weather conditions