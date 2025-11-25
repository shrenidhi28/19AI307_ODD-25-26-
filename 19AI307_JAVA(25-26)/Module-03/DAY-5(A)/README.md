# Ex.No:3(E) INNER CLASS

## QUESTION: Write a Java program where the inner class is declared private and accessed through a method in the outer class. 


## AIM: To demonstrate the use of a private inner class in Java and how it can be accessed through a method in the outer class.


## ALGORITHM :
1. Start the program.
2. Import the required package `java.util`.
3. Define the outer class.
4. Create a private inner class inside the outer class.
5. Declare a private variable and a private method inside the inner class.
6. Create a public method in the outer class to access the private inner class.
7. In the main method, read input from the user.
8. Create an instance of the outer class.
9. Call the method that accesses the private inner class and pass the input value.
10. End the program.
	





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: 
RegisterNumber:
import java.util.*;
public class Main{
    private class Inner{
        private int data;
        private void setData(int value){
            data = value;
            System.out.println("Data set inside private inner class: " + data);
        }
    }
    public void accessInner(int value){
        Inner inner = new Inner();
        inner.setData(value);
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        Main outer = new Main();
        outer.accessInner(num);
    }
} 
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Main{
    private class Inner{
        private int data;
        private void setData(int value){
            data = value;
            System.out.println("Data set inside private inner class: " + data);
        }
    }
    public void accessInner(int value){
        Inner inner = new Inner();
        inner.setData(value);
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        Main outer = new Main();
        outer.accessInner(num);
    }
}
```







## OUTPUT:
<img width="829" height="278" alt="image" src="https://github.com/user-attachments/assets/bf561d9f-ba5d-4c7e-b6b8-6573b2c9d674" />




## RESULT:
Thus, the Java program successfully demonstrated a private inner class being accessed through a method in the outer class.
