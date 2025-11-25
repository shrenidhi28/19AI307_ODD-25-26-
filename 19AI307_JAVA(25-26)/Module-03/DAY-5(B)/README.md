# Ex.No:3(F) WRAPPER CLASS

## QUESTION: Find the largest digit in a number using wrapper class methods.


## AIM: To write a Java program that finds the largest digit in a given number using wrapper class methods such as Integer.toString() and Character.getNumericValue().


## ALGORITHM :
1. Start the program.
2. Import the required package `java.util`.
3. Read the number from the user.
4. Convert the number to a string using `Integer.toString()`.
5. Initialize a variable to store the largest digit.
6. Loop through each character in the string.
7. Convert each character to a digit using `Character.getNumericValue()`.
8. Compare the digit with the current maximum and update if larger.
9. Display the largest digit.
10. End the program.





## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: 
RegisterNumber:
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        String str = Integer.toString(num);  // Wrapper class method
        int maxDigit = 0;

        for (int i = 0; i < str.length(); i++) {
            int digit = Character.getNumericValue(str.charAt(i)); // Wrapper method
            if (digit > maxDigit) {
                maxDigit = digit;
            }
        }

        System.out.println("Largest Digit: " + maxDigit);
    }
}

*/
```

## SOURCE CODE:

```
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        String str = Integer.toString(num);  // Wrapper class method
        int maxDigit = 0;

        for (int i = 0; i < str.length(); i++) {
            int digit = Character.getNumericValue(str.charAt(i)); // Wrapper method
            if (digit > maxDigit) {
                maxDigit = digit;
            }
        }

        System.out.println("Largest Digit: " + maxDigit);
    }
} 
```





## OUTPUT:
<img width="829" height="237" alt="image" src="https://github.com/user-attachments/assets/138668e4-8372-447a-901d-32fd5202fe5f" />



## RESULT:
Thus, the Java program to find the largest digit in a number using wrapper class methods was executed successfully.

