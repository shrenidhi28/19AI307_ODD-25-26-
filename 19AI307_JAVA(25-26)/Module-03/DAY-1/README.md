# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION: Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade 


## AIM: To implement Inheritance and understand how subclass extends the functionality of a superclass in Java by adding additional fields and methods.


## ALGORITHM :
1. Start the program.
2. Import the required package `java.util.Scanner`.
3. Create a superclass `Person` with fields:
   - `name`
   - `age`
4. Create a subclass `Student` that extends `Person` and adds:
   - `mark`
   - A method `calculateGrade()` to determine grade based on marks.
5. In the `main()` method:
   - Create a `Student` object.
   - Read the student's name, age, and mark using Scanner.
   - Display the name, age, and mark.
   - Call `calculateGrade()` to print the grade.
6. End the program.






## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.*;
class Person{
    String name;
    int age;
}
class Student extends Person{
    int mark;
    String calculateGrade(){
        if(mark>=90){
            return "Grade: A" ;
        }
        else if(mark>=75 && mark<90){
            return "Grade: B" ;
        }
        else if(mark >=50 && mark < 75){
            return "Grade: C" ;
        }
        else{
            return "Grade: F" ;
        }
    }
}
public class Main{
    public static void main(String [] args){
        Student obj = new Student();
        Scanner sc = new Scanner(System.in);
        
        obj.name = sc.nextLine();
        //sc.nextLine();
        obj.age = sc.nextInt();
        obj.mark = sc.nextInt();
        System.out.println("Name: " + obj.name);
        System.out.println("Age: " + obj.age);
        System.out.println("Marks: " + obj.mark);
        System.out.println(obj.calculateGrade());
        
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;
class Person{
    String name;
    int age;
}
class Student extends Person{
    int mark;
    String calculateGrade(){
        if(mark>=90){
            return "Grade: A" ;
        }
        else if(mark>=75 && mark<90){
            return "Grade: B" ;
        }
        else if(mark >=50 && mark < 75){
            return "Grade: C" ;
        }
        else{
            return "Grade: F" ;
        }
    }
}
public class Main{
    public static void main(String [] args){
        Student obj = new Student();
        Scanner sc = new Scanner(System.in);
        
        obj.name = sc.nextLine();
        //sc.nextLine();
        obj.age = sc.nextInt();
        obj.mark = sc.nextInt();
        System.out.println("Name: " + obj.name);
        System.out.println("Age: " + obj.age);
        System.out.println("Marks: " + obj.mark);
        System.out.println(obj.calculateGrade());
        
    }
}
```






## OUTPUT:
<img width="467" height="537" alt="image" src="https://github.com/user-attachments/assets/e8546a12-8fbf-4fdd-bea5-826191dbc5c7" />




## RESULT:
Thus, the Java program implementing Inheritance and Aggregation using Person and Student classes was executed successfully.

