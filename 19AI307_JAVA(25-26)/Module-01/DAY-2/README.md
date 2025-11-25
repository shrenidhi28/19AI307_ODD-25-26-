# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION: Write a Java program to simulate this elevator logic for a given floor number.


## AIM: To Write a Java program to simulate this elevator logic for a given floor number.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Read the input floor number from the user.

4.Check if the number is divisible by both 3 and 5. If true, print "Skipped".

5.Else if the number is divisible by 3, print "Beware!".

6.Else if the number is divisible by 5, print "Blessings!".

7.Else, print "Floor {number}".	





## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196

import java.util.Scanner;
public class main{
    public static void main(String args[]){
        int a;
        Scanner sc = new Scanner(System.in);
        a=sc.nextInt();
        
        if(a%3==0 && a%5==0){
            System.out.println("Skipped");
        }
        else if(a%3==0){
            System.out.println("Beware!");
        }
        else if(a%5==0){
            System.out.println("Blessings!");
        }
        else{
            System.out.println("Floor " + a);
        }
        
        
    }
}
*/
```

## SOURCE CODE:


```
import java.util.Scanner;
public class main{
    public static void main(String args[]){
        int a;
        Scanner sc = new Scanner(System.in);
        a=sc.nextInt();
        
        if(a%3==0 && a%5==0){
            System.out.println("Skipped");
        }
        else if(a%3==0){
            System.out.println("Beware!");
        }
        else if(a%5==0){
            System.out.println("Blessings!");
        }
        else{
            System.out.println("Floor " + a);
        }
        
        
    }
}

```







## OUTPUT:


<img width="877" height="276" alt="image" src="https://github.com/user-attachments/assets/97cb2a93-bdbb-49c0-b6c2-19cbc1723759" />


## RESULT:

Thus, the Java program to simulate the elevator logic using conditional statements was successfully executed and verified.

