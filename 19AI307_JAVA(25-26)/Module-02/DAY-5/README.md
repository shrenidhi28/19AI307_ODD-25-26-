# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION: Create a class Calculator with: One non-static method add(int a, int b) that returns the sum, One static method info() that says "Calculator is ready".


## AIM: To write a Java program that demonstrates the use of access modifiers, static methods, and non-static methods using a Calculator class.


## Algorithm

1. Start the program.
2. Import the required package `java.util.Scanner`.
3. Create a class `Calculator` with:
   - A non-static method `add(int a, int b)` that returns the sum.
   - A static method `info()` that prints "Calculator is ready".
4. In the `main()` method (inside class `prog`):
   - Create a `Scanner` object to read two integers from the user.
   - Call the static method `Calculator.info()` to display the message.
   - Create an object of the `Calculator` class.
   - Call the `add()` method using the object to compute the sum.
   - Display the result.
5. End the program.
	





## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by:  Shrenidhi C
RegisterNumber: 212223040196
import java.util.Scanner;

class Calculator {
   // Your Methods here
   public int add (int a ,int b){
       return a+b;
   }
   public static void info(){
       System.out.println( "Calculator is ready");
   }
}

class prog {
    public static void main(String[] args) {
         // Your Function Initiation here
         int a ,b;
         Scanner sc = new Scanner(System.in);
         a = sc.nextInt();
         b = sc.nextInt();
         Calculator.info();
         
         Calculator obj = new Calculator();
         System.out.print("Sum: " + obj.add(a,b));
    }
}
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Calculator {
   // Your Methods here
   public int add (int a ,int b){
       return a+b;
   }
   public static void info(){
       System.out.println( "Calculator is ready");
   }
}

class prog {
    public static void main(String[] args) {
         // Your Function Initiation here
         int a ,b;
         Scanner sc = new Scanner(System.in);
         a = sc.nextInt();
         b = sc.nextInt();
         Calculator.info();
         
         Calculator obj = new Calculator();
         System.out.print("Sum: " + obj.add(a,b));
    }
}
```






## OUTPUT:
<img width="881" height="281" alt="image" src="https://github.com/user-attachments/assets/bd86d878-f926-4397-9b72-0cb0fae4ec63" />



## RESULT:
Thus, the program demonstrating access modifiers using static and non-static methods in the Calculator class was successfully executed.
