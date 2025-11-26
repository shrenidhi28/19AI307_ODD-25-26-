# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION: Write a Java program to write characters to a file using FileWriter.


## AIM: To write character data to a file in Java using the `FileWriter` class.


## ALGORITHM :
1. Start the program.  
2. Import the necessary packages: `java.io.FileWriter`, `java.io.IOException`, `java.util.Scanner`.  
3. Create a `Scanner` object to accept user input for the file name and data to write.  
4. Create a `FileWriter` object with the given file name.  
5. Use the `write()` method of `FileWriter` to write the input data to the file.  
6. Display a success message: `"File written successfully."`  
7. Close the `FileWriter` object to save and release resources.  
8. End the program.






## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: Shrenidhi 
RegisterNumber:212223040196
import java.io.FileWriter;
import java.io.IOException;
import java.util.Scanner;

public class WriteFileUsingFileWriter {
    public static void main(String[] args) throws IOException {
    //write your code here
    
    Scanner sc = new Scanner(System.in);
    String name = sc.nextLine();
    String data = sc.nextLine();
    FileWriter fos = new FileWriter(name);
    
    fos.write(data);
    System.out.println("File written successfully.");
    fos.close();
    
    
    
    
    
    }
}

*/
```

## SOURCE CODE:

```
import java.io.FileWriter;
import java.io.IOException;
import java.util.Scanner;

public class WriteFileUsingFileWriter {
    public static void main(String[] args) throws IOException {
    //write your code here
    
    Scanner sc = new Scanner(System.in);
    String name = sc.nextLine();
    String data = sc.nextLine();
    FileWriter fos = new FileWriter(name);
    
    fos.write(data);
    System.out.println("File written successfully.");
    fos.close();
    
    
    
    
    
    }
}

```






## OUTPUT:
<img width="961" height="363" alt="image" src="https://github.com/user-attachments/assets/906c0d31-35a0-4dd4-8652-df59cc11d8a7" />




## RESULT:

The program successfully writes the input data to a file using FileWriter in Java.
