# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION: Write a program to overwrite the content of a file.


## AIM: To demonstrate **file handling in Java** by overwriting the content of an existing file using `FileWriter`.


## ALGORITHM :
1. Start the program.  
2. Import the necessary packages: `java.util.*`, `java.io.*`.  
3. Create a `Scanner` object to accept user input for the new file content.  
4. Create a `FileWriter` object with the target file name (`input.txt`).  
5. Use the `write()` method of `FileWriter` to overwrite the existing file content.  
6. Display a success message: `"File content overwritten successfully."`  
7. Close the `FileWriter` to save changes and release resources.  
8. End the program.






## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.*;
import java.io.*;
public class Main{
    public static void main(String[] args) throws Exception{
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        FileWriter obj = new FileWriter("input.txt");
        obj.write(a);
        System.out.println("File content overwritten successfully.");
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
import java.io.*;
public class Main{
    public static void main(String[] args) throws Exception{
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        FileWriter obj = new FileWriter("input.txt");
        obj.write(a);
        System.out.println("File content overwritten successfully.");
    }
}
```







## OUTPUT:
<img width="961" height="265" alt="image" src="https://github.com/user-attachments/assets/b854358e-61ff-429a-be1f-ee5c948b29b8" />




## RESULT:

The program successfully demonstrates file handling in Java

