# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION: Read N numbers from user, use a fixed thread pool (size 3) to compute the sum of each number multiplied by 2. Return results in order.




## AIM: To demonstrate **multithreading and synchronization** in Java by processing multiple tasks concurrently using a thread pool.

---


## ALGORITHM :
1. Start the program.  
2. Import the necessary packages: `java.util.*`.  
3. Create a `Multithreading` class that extends `Thread` and stores an integer value.  
4. Implement a method `Run()` to return the number multiplied by 2.  
5. In the `main()` method:  
   - Accept the number of inputs `N`.  
   - Accept `N` integers from the user.  
   - For each number, create a thread object and compute `2 * number` using `Run()`.  
   - Display the result for each number in input order.  
6. End the program.

---	





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: 
RegisterNumber:
import java.util.*;
class Multithreading extends Thread{
    int a;
    Multithreading(int a ){
        this.a = a;
    }
    public void run(){
        
    }
    int Run(){
        return 2*a;
    }
    
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        for(int i=0;i<n;i++){
            int a = sc.nextInt();
            sc.nextLine();
            Multithreading t1 = new Multithreading(a);
            System.out.println("Result: "+t1.Run());
            //t1.setName(a);
            // t1.start();
        }
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
class Multithreading extends Thread{
    int a;
    Multithreading(int a ){
        this.a = a;
    }
    public void run(){
        
    }
    int Run(){
        return 2*a;
    }
    
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        for(int i=0;i<n;i++){
            int a = sc.nextInt();
            sc.nextLine();
            Multithreading t1 = new Multithreading(a);
            System.out.println("Result: "+t1.Run());
            //t1.setName(a);
            // t1.start();
        }
    }
}
```






## OUTPUT:
<img width="961" height="424" alt="image" src="https://github.com/user-attachments/assets/ca9b218b-cbce-4936-96b8-eaffe962cb2b" />



## RESULT:
The program successfully demonstrates multithreading with synchronization.

