# Ex.No:3(b) POLYMORPHISM

## QUESTION: Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator


## AIM: To implement compile-time polymorphism (method overloading) in Java by defining multiple area() methods with different parameter lists to calculate the area of various shapes.


## ALGORITHM :
1. Start the program.
2. Import the package `java.util.Scanner`.
3. Create a class `AreaCalculator` with overloaded `area()` methods.
4. Define `area(int side)` to calculate the area of a square.
5. Define `area(int length, int breadth)` to calculate the area of a rectangle.
6. Define `area(double radius)` to calculate the area of a circle.
7. In the `main()` method, create a Scanner object to read inputs.
8. Create an object of the `AreaCalculator` class.
9. Read values for side, length, breadth, and radius from the user.
10. Call the correct overloaded `area()` method based on input type.
11. Print the calculated areas for square, rectangle, and circle.
12. End the program.





## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: shrenidhi C
RegisterNumber: 212223040196
import java.util.*;
class AreaCalculator{
    int area(int side){
        return side*side;
        
    }
    int area(int l, int b){
        return l*b ;
        
    }
    double area(double radius){
        return (Math.PI * radius *radius);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc  = new Scanner(System.in);
        AreaCalculator obj = new  AreaCalculator();
        int s,l,b;
        double r;
        s = sc.nextInt();
        l= sc.nextInt();
        b= sc.nextInt();
        r = sc.nextDouble();
        System.out.println("Area of square: "+ obj.area(s));
        System.out.println("Area of rectangle: "+ obj.area(l,b));
        System.out.println("Area of circle: "+ obj.area(r));
        
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
class AreaCalculator{
    int area(int side){
        return side*side;
        
    }
    int area(int l, int b){
        return l*b ;
        
    }
    double area(double radius){
        return (Math.PI * radius *radius);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc  = new Scanner(System.in);
        AreaCalculator obj = new  AreaCalculator();
        int s,l,b;
        double r;
        s = sc.nextInt();
        l= sc.nextInt();
        b= sc.nextInt();
        r = sc.nextDouble();
        System.out.println("Area of square: "+ obj.area(s));
        System.out.println("Area of rectangle: "+ obj.area(l,b));
        System.out.println("Area of circle: "+ obj.area(r));
        
    }
}
```







## OUTPUT:
<img width="829" height="386" alt="image" src="https://github.com/user-attachments/assets/37dcf1c1-a2a5-487a-b921-0471cc77455c" />



## RESULT:
Thus, the Java program demonstrating Polymorphism through Method Overloading was successfully executed.

