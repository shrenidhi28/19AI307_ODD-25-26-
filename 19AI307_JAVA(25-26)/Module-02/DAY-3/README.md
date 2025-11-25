# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION: Write a Java program to create a class called “Book” with private instance variables title, author, and price. Provide public getter and setter methods to access and modify these variables. Add a method called applyDiscount() that takes a percentage as a parameter and reduces the price by that percentage.


## AIM: To write a Java program that demonstrates the use of access specifiers by defining private data members and accessing them using public getter and setter methods.


## ALGORITHM :
1.Start the program.

2.Import the necessary package java.util.

3.Create a class Book with private variables title, author, and price.

4.Create public getter and setter methods for each variable.

5.Define a method applyDiscount() to reduce the price by a given percentage.

6.In the main method, read user inputs for title, author, price, and discount percentage.

7.Create a Book object and set the values using setter methods.

8.Apply the discount and display the updated details.

9.End the program.





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.Scanner;

class Book {
    private String title;
    private String author;
    private double price;

    
    public String getTitle() {
        return title;
    }

    public String getAuthor() {
        return author;
    }

    public double getPrice() {
        return price;
    }


    public void setTitle(String title) {
        this.title = title;
    }

    public void setAuthor(String author) {
        this.author = author;
    }

    public void setPrice(double price) {
        this.price = price;
    }

   
    public void applyDiscount(double percentage) {
        if (percentage > 0 && percentage <= 100) {
            price = price - (price * (percentage / 100));
        }
    }

  
    public void display() {
        System.out.println("Title: " + title);
        System.out.println("Author: " + author);
        System.out.printf("Discounted Price: %.2f\n", price);
        System.out.println("-------------------------");
    }
}
public class Main{
    public static void main(String[] args){
        String Title, author;
        double price,per;
        Scanner sc = new Scanner(System.in);
        Title = sc.nextLine();
        author = sc.nextLine();
        price = sc.nextDouble();
        per = sc.nextDouble();
        
        Book obj = new Book();
        obj.setTitle(Title);
        obj.setAuthor(author);
        obj.setPrice(price);
        obj.applyDiscount(per);
        obj.display();
    }
}
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Book {
    private String title;
    private String author;
    private double price;

    
    public String getTitle() {
        return title;
    }

    public String getAuthor() {
        return author;
    }

    public double getPrice() {
        return price;
    }


    public void setTitle(String title) {
        this.title = title;
    }

    public void setAuthor(String author) {
        this.author = author;
    }

    public void setPrice(double price) {
        this.price = price;
    }

   
    public void applyDiscount(double percentage) {
        if (percentage > 0 && percentage <= 100) {
            price = price - (price * (percentage / 100));
        }
    }

  
    public void display() {
        System.out.println("Title: " + title);
        System.out.println("Author: " + author);
        System.out.printf("Discounted Price: %.2f\n", price);
        System.out.println("-------------------------");
    }
}
public class Main{
    public static void main(String[] args){
        String Title, author;
        double price,per;
        Scanner sc = new Scanner(System.in);
        Title = sc.nextLine();
        author = sc.nextLine();
        price = sc.nextDouble();
        per = sc.nextDouble();
        
        Book obj = new Book();
        obj.setTitle(Title);
        obj.setAuthor(author);
        obj.setPrice(price);
        obj.applyDiscount(per);
        obj.display();
    }
}

```






## OUTPUT:
<img width="881" height="524" alt="image" src="https://github.com/user-attachments/assets/8e4695d0-fb7d-4cb3-83ad-9f69adc03fc0" />



## RESULT:
Thus, the Java program implementing access specifiers using private variables with public getter, setter, and discount methods was successfully executed and verified.

