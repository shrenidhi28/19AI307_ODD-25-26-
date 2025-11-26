# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION: You are asked to simulate a simple Shape Drawing Tool using the Factory Design Pattern in Java.




## AIM:


## Algorithm

1. Start the program.  
2. Import the necessary package `java.util.*`.  
3. Create a `Shape` interface with a method `draw()`.  
4. Implement concrete classes `Circle`, `Square`, and `Rectangle` that implement the `Shape` interface.  
5. Create a `ShapeFactory` class with a method `give(String shapeType)` that returns the appropriate Shape object based on input.  
   - If the input is `"circle"`, return a `Circle` object.  
   - If the input is `"square"`, return a `Square` object.  
   - If the input is `"rectangle"`, return a `Rectangle` object.  
   - If the input is invalid, display an error message and return `null`.  
6. In the `main()` method, create a `Scanner` object to accept user input.  
7. Continuously read input until the user enters `"exit"`.  
8. For each input, use the `ShapeFactory` to get the appropriate Shape object.  
9. If the Shape object is not `null`, call its `draw()` method to display the drawing.  
10. End the program when the user types `"exit"`.  






## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: 
RegisterNumber:
import java.util.*;

interface Shape{
    void draw();
}
class Circle implements Shape{
    public void draw(){
        System.out.println("Drawing Circle");
    }
    
}
class Square implements Shape{
    public void draw(){
        System.out.println("Drawing Square");
    }
    
}
class Rectangle implements Shape{
    public void draw(){
        System.out.println("Drawing Rectangle");
    }
    
}
class ShapeFactory{
    Shape give(String a){
        if(a.equalsIgnoreCase("circle")){
            return (new Circle()); //objc
        }
        else if(a.equalsIgnoreCase("square")){
            return (new Square());
        }
        else if(a.equalsIgnoreCase("rectangle")){
            return (new Rectangle());
        }
        else{
            System.out.println("Invalid shape: "+ a);
            return null;
        }
    }
    
}

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        
        while(sc.hasNextLine()){
            String a = sc.nextLine();
            if(a.equalsIgnoreCase("exit")){
                break;
            }
            ShapeFactory obj = new ShapeFactory();
            Shape objc =obj.give(a);
            if(objc!=null)
                objc.draw();
            
            
        }
    }
}
*/
```

## SOURCE CODE:

```
import java.util.*;

interface Shape{
    void draw();
}
class Circle implements Shape{
    public void draw(){
        System.out.println("Drawing Circle");
    }
    
}
class Square implements Shape{
    public void draw(){
        System.out.println("Drawing Square");
    }
    
}
class Rectangle implements Shape{
    public void draw(){
        System.out.println("Drawing Rectangle");
    }
    
}
class ShapeFactory{
    Shape give(String a){
        if(a.equalsIgnoreCase("circle")){
            return (new Circle()); //objc
        }
        else if(a.equalsIgnoreCase("square")){
            return (new Square());
        }
        else if(a.equalsIgnoreCase("rectangle")){
            return (new Rectangle());
        }
        else{
            System.out.println("Invalid shape: "+ a);
            return null;
        }
    }
    
}

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        
        while(sc.hasNextLine()){
            String a = sc.nextLine();
            if(a.equalsIgnoreCase("exit")){
                break;
            }
            ShapeFactory obj = new ShapeFactory();
            Shape objc =obj.give(a);
            if(objc!=null)
                objc.draw();
            
            
        }
    }
}
```






## OUTPUT:
<img width="961" height="449" alt="image" src="https://github.com/user-attachments/assets/be1d9695-2255-4daa-8743-de9bf5ca38da" />




## RESULT:
The program successfully demonstrates the Abstract Factory Design Pattern.

