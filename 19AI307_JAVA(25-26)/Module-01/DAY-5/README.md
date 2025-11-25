# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION: Write a Java program to reverse a given string.


## AIM: To write a Java program that reads a string and prints its reverse using string functions.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Read a string from the user.

4.Find the length of the string.

5.Traverse the string in reverse order using a loop.

6.Print each character from the end to the beginning.

7.End the program.




## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196

import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String str = new String();
        str=sc.next();
        int length=str.length()-1;
        // System.out.print(str);
        System.out.print("Reversed string: ");
        for(int i=length;i>=0;i--){
            char a=str.charAt(i);
            System.out.print(a);
        }
    }
}
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String str = new String();
        str=sc.next();
        int length=str.length()-1;
        // System.out.print(str);
        System.out.print("Reversed string: ");
        for(int i=length;i>=0;i--){
            char a=str.charAt(i);
            System.out.print(a);
        }
    }
}

```







## OUTPUT:
<img width="719" height="270" alt="image" src="https://github.com/user-attachments/assets/5ecdff55-633a-46fe-8534-a2c53826e757" />




## RESULT:
Thus, the Java program to reverse a given string was successfully executed and verified.

