# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION: Write a program that reads two integers and divides the first by the second. Handle the case when division by zero occurs.


## AIM: To write a Java program that reads two integers from the user and performs division while handling the division-by-zero exception using try-catch blocks.



## ALGORITHM :
1. Start the program.
2. Import the required package `java.util`.
3. Read two integers from the user.
4. Use a try block to perform division of the first integer by the second.
5. If division is successful, display the result.
6. If an ArithmeticException occurs (division by zero), catch it and display an error message.
7. End the program.






## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        try{
            int n = a/b;
            System.out.println("Result: " + n);
        }
        catch(ArithmeticException e){
            System.out.println("Error: Division by zero");
        }
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        try{
            int n = a/b;
            System.out.println("Result: " + n);
        }
        catch(ArithmeticException e){
            System.out.println("Error: Division by zero");
        }
    }
}

```






## OUTPUT:

<img width="755" height="333" alt="image" src="https://github.com/user-attachments/assets/c18b8ca9-16f2-416c-92f8-95d157172e71" />


## RESULT:
Thus, the Java program to handle division by zero using exception handling was successfully implemented and executed.

