# Ex.No:1(D) ARRAYS

## QUESTION: Write a Java Program to Find the Average of Array Elements.


## AIM: To write a Java program that reads an array of numbers and calculates the average of its elements.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Read the number of elements n from the user.

4.Declare an array of size n.

5.Read each array element inside a loop.

6.Calculate the sum of all elements.

7.Compute the average as sum / n.

8.Display the average value.

9.End the program.




## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196

import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        float sum=0;
        int arr[] =new int[n] ;
        for(int i =0;i<n;i++){
            arr[i]=sc.nextInt();
            sum=sum+arr[i];
        }
        float res=sum/n;
        System.out.printf("The average of elements is %.2f" , res);
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
        int n = sc.nextInt();
        float sum=0;
        int arr[] =new int[n] ;
        for(int i =0;i<n;i++){
            arr[i]=sc.nextInt();
            sum=sum+arr[i];
        }
        float res=sum/n;
        System.out.printf("The average of elements is %.2f" , res);
    }
}

```






## OUTPUT:
<img width="719" height="452" alt="image" src="https://github.com/user-attachments/assets/e044fc43-1782-4cf3-aa9f-5761434b8bdf" />



## RESULT:
Thus, the Java program to find the average of array elements was successfully executed and verified.

