# Ex.No:1(C) LOOPING STATEMENT

## QUESTION: Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.


## AIM: To write a Java program to calculate the factorial of a given number using a for loop.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Read the integer input n from the user.

4.Initialize a variable res to 1.

5.Use a for loop from 1 to n and multiply res by each value.

6.Display the factorial result.

7.End the program.





## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: ShrenidhiC
RegisterNumber: 212223040196

 import java.util.Scanner;
public class main{
    public static void main(String a[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int res=1;
        for(int i=1;i<=n;i++){
            res=res*i;
        }
        System.out.print("Factorial of "+n+" is: "+res);
    }
}
*/
```

## SOURCE CODE:

```

import java.util.Scanner;
public class main{
    public static void main(String a[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int res=1;
        for(int i=1;i<=n;i++){
            res=res*i;
        }
        System.out.print("Factorial of "+n+" is: "+res);
    }
}

```




## OUTPUT:

<img width="877" height="276" alt="image" src="https://github.com/user-attachments/assets/38788985-e83d-4418-858e-756e10e941a9" />



## RESULT:
Thus, the Java program to calculate the factorial of a number using a for loop was successfully executed and verified.
