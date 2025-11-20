# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Synchronize deposit method in a BankAccount class, simulate deposits from multiple threads.

## AIM:

To write a Java program that demonstrates multithreading with synchronization by simulating multiple deposit operations on a shared bank account.

## ALGORITHM :

1. Define a class BankAccount with:
    * A private variable balance.
    * A synchronized method deposit(int amount) that adds the amount to the balance.
    * A method getBalance() to return the current balance.
2. Define a class DepositThread that extends Thread:
    * Store references to a BankAccount object and deposit amount.
    * In the run() method, call account.deposit(amount).
3. In the main method:
    * Create a Scanner object to read input.
    * Read the number of deposit operations n.
    * Create an array of Thread objects.
    * For each deposit, read the amount and create a DepositThread object.
    * Start all threads.
    * Use join() to ensure all threads finish execution.
    * Print the final balance using getBalance().
4. End the program.




## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:

```java
import java.util.*;
class BankAccount{
    private int balance = 0;
    
    public synchronized void deposit(int amount){
        balance += amount;
    }
    
    public int getBalance(){
        return balance;
    }
}

class DepositThread extends Thread{
    private BankAccount account;
    private int amount;
    
    DepositThread(BankAccount account, int amount){
        this.account = account;
        this.amount = amount;
    }
    
    public void run(){
        account.deposit(amount);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int  n = sc.nextInt();
        
        Thread[] threads = new Thread[n];
        BankAccount account = new BankAccount();
        
        for(int i=0;i<n;i++){
            int amount = sc.nextInt();
            threads[i] = new DepositThread(account,amount);
        }
        
        for(int i=0;i<n;i++){
            threads[i].start();
        }
        
        for(int i=0;i<n;i++){
            try{
                threads[i].join();
            }
            catch(InterruptedException e){
                System.out.print(e.getMessage());
            }
        }
        
        System.out.println("Final Balance: " + account.getBalance());
    }
}
```





## OUTPUT:

![alt text](image.png)

## RESULT:

The program successfully demonstrates thread synchronization ensuring consistent updates to the shared balance.
