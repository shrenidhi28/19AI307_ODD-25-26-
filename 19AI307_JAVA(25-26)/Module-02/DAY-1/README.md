# Ex.No:2(A) CLASS AND OBJECT

## QUESTION: Create a class Car with attributes brand, model, year. Create 2 objects and print their details.


## AIM: To write a Java program that creates a Car class with attributes and demonstrates object creation by printing details of two car objects.


## ALGORITHM :
1.Start the program.

2.Create a class Car with data members brand, model, and year.

3.Inside the main method, create two objects of the Car class.

4.Assign values to the attributes of each object.

5.Print the details of both car objects.

6.End the program.




## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
public class prog {
    public static class Car{
        String brand,model;
        int year;
    }
    
    public static void main(String[] args) {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}

*/
```

## SOURCE CODE:

```

    
public class prog {
    public static class Car{
        String brand,model;
        int year;
    }
    
    public static void main(String[] args) {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}


```






## OUTPUT:

<img width="719" height="270" alt="image" src="https://github.com/user-attachments/assets/f3289d55-5ef2-47c8-95bd-e4c7a1f73769" />


## RESULT:
Thus, the Java program to create a class with attributes and print the details of two car objects was successfully executed and verified.
