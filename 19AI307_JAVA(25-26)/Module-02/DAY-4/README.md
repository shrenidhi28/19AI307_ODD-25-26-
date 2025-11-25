# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION: Write a program to access a static variable using both class name and object.


## AIM:To write a Java program that demonstrates accessing a static variable using both the class name and an object of the class.


## Algorithm

1. Start the program.
2. Import the required package `java.util.Scanner`.
3. Create a class `Demo` and declare a static variable `num`.
4. In the `main()` method, create a `Scanner` object to read input from the user.
5. Assign the input value to the static variable using the class name (`Demo.num`).
6. Print the value of the static variable using the class name.
7. Create an object of the `Demo` class.
8. Access and print the static variable using the object.
9. End the program.






## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.Scanner;

class Demo {
    // static variable
    static int num;
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        // take input
        Demo.num = sc.nextInt();
        
        // accessing using class name
        System.out.println("Accessing using class name: " + Demo.num);
        
        // creating object
        Demo obj = new Demo();
        
        // accessing using object
        System.out.println("Accessing using object: " + obj.num);
        
        sc.close();
    }
}

*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Demo {
    // static variable
    static int num;
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        // take input
        Demo.num = sc.nextInt();
        
        // accessing using class name
        System.out.println("Accessing using class name: " + Demo.num);
        
        // creating object
        Demo obj = new Demo();
        
        // accessing using object
        System.out.println("Accessing using object: " + obj.num);
        
        sc.close();
    }
}

```






## OUTPUT:
<img width="881" height="281" alt="image" src="https://github.com/user-attachments/assets/4426fe36-9508-44cb-8a08-2b492e2dd85e" />



## RESULT: 
Thus, the Java program to access a static variable using both class name and object was executed successfully.

