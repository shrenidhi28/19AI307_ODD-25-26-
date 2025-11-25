# Ex.No:2(B) METHODS

## QUESTION: Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).




## AIM: To write a Java program that demonstrates method calling by defining a square() method and using it inside a cube() method.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Create a class containing two methods: square(int) and cube(int).

4.The cube(int) method should call square(int) internally.

5.In the main method, read an integer from the user.

6.Create an object and call the cube() method.

7.Display the result.

8.End the program.	





## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.Scanner;
public class Main{
    public static class Cube{
        //non static - needs the help of obj to be called 
        int square(int x){
            return x*x;
        }
        int cube(int x){
            return x*square(x);
        }
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        Cube obj1 = new Cube();
        int x = sc.nextInt();
        System.out.print(obj1.cube(x));
    }
}
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Main{
    public static class Cube{
        //non static - needs the help of obj to be called 
        int square(int x){
            return x*x;
        }
        int cube(int x){
            return x*square(x);
        }
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        Cube obj1 = new Cube();
        int x = sc.nextInt();
        System.out.print(obj1.cube(x));
    }
}

```





## OUTPUT:

<img width="719" height="233" alt="image" src="https://github.com/user-attachments/assets/ad187379-736e-4e0e-9faf-517fcd7bf30f" />


## RESULT:
Thus, the Java program demonstrating method calling using square() inside cube() was successfully executed and verified.

