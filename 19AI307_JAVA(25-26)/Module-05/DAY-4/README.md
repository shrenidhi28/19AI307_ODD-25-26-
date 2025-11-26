# Ex.No:5(D) THREAD PRIORITY

## QUESTION: Write a java program for set the priority and name of the current thread.Consider two threads t1 and t2


## AIM: To demonstrate **thread naming and priority** in Java using the `Thread` class.

---


## ALGORITHM :
1. Start the program.  
2. Import the necessary package: `java.util.*`.  
3. Create a class `Multithreading` that extends `Thread`.  
4. In the `main()` method:  
   - Accept two thread names from the user.  
   - Create two thread objects: `t1` and `t2`.  
   - Set the name and priority for each thread using `setName()` and `setPriority()`.  
   - Display the thread details (name, priority, and state) on the console.  
5. End the program.





## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.*;
class Multithreading extends Thread{
    public void run(){
        // System.out.println("Thread[" + getName() + "," + getPriority() +",main]");
    }
}

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        String b = sc.nextLine();
        Multithreading t1 = new Multithreading();
        Multithreading t2 = new Multithreading();
        
        t1.setName(a);
        t1.setPriority(4);
        //t1.start();
        
        t2.setName(b);
        t2.setPriority(2);
        //t2.start();
        System.out.println("Thread[" + t1.getName() + "," + t1.getPriority() +",main]");
        System.out.println("Thread[" + t2.getName() + "," + t2.getPriority() +",main]");
    
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
class Multithreading extends Thread{
    public void run(){
        // System.out.println("Thread[" + getName() + "," + getPriority() +",main]");
    }
}

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        String b = sc.nextLine();
        Multithreading t1 = new Multithreading();
        Multithreading t2 = new Multithreading();
        
        t1.setName(a);
        t1.setPriority(4);
        //t1.start();
        
        t2.setName(b);
        t2.setPriority(2);
        //t2.start();
        System.out.println("Thread[" + t1.getName() + "," + t1.getPriority() +",main]");
        System.out.println("Thread[" + t2.getName() + "," + t2.getPriority() +",main]");
    
    }
}
```






## OUTPUT:
<img width="961" height="265" alt="image" src="https://github.com/user-attachments/assets/bb3acd9e-6493-4abf-a68c-e08e259b9253" />




## RESULT: 
The program successfully demonstrates thread naming and priority in Java.

