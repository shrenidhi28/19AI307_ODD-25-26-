# Ex.No:3(C) ABSTRACTION

## QUESTION: Create an abstract class Employee with method calculatePay(). Extend it to HourlyEmployee and SalariedEmployee.


## AIM: To implement abstraction in Java using abstract classes and method overriding in subclasses.


## ALGORITHM :
1. Start the program.
2. Import the package `java.util.Scanner`.
3. Create an abstract class `Employee` with an abstract method `calculatePay()`.
4. Create a subclass `HourlyEmployee` extending `Employee`.
5. Add fields `hoursWorked` and `ratePerHour` to `HourlyEmployee`.
6. Implement `calculatePay()` in `HourlyEmployee` to return hoursWorked * ratePerHour.
7. Create another subclass `SalariedEmployee` extending `Employee`.
8. Add a field `monthlySalary` to `SalariedEmployee`.
9. Implement `calculatePay()` in `SalariedEmployee` to return monthlySalary.
10. In the `main()` method, create a Scanner object to read user input.
11. Read user choice (1 for hourly, 2 for salaried).
12. If choice is hourly, read hours and rate, then create an HourlyEmployee object.
13. If choice is salaried, read salary and create a SalariedEmployee object.
14. Call `calculatePay()` on the created object.
15. Print the calculated pay.
16. End the program.





## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: Shrenidhi C
RegisterNumber: 212223040196
import java.util.*;

abstract class Employee {
    abstract double calculatePay();
}

class HourlyEmployee extends Employee {
    private int hoursWorked;
    private double ratePerHour;

    HourlyEmployee(int hoursWorked, double ratePerHour) {
        this.hoursWorked = hoursWorked;
        this.ratePerHour = ratePerHour;
    }

    @Override
    double calculatePay() {
        return hoursWorked * ratePerHour;
    }
}

class SalariedEmployee extends Employee {
    private double monthlySalary;

    SalariedEmployee(double monthlySalary) {
        this.monthlySalary = monthlySalary;
    }

    @Override
    double calculatePay() {
        return monthlySalary;
    }
}

public class EmployeePayCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice = sc.nextInt();
        Employee emp;
        if (choice == 1) {
            int hours = sc.nextInt();
            double rate = sc.nextDouble();
            emp = new HourlyEmployee(hours, rate);
        } else if (choice == 2) {
            double salary = sc.nextDouble();
            emp = new SalariedEmployee(salary);
        } else {
            System.out.println("Invalid choice");
            sc.close();
            return;
        }
        System.out.printf("%.2f%n", emp.calculatePay());
        sc.close();
    }
}

*/
```

## SOURCE CODE:


```
import java.util.*;

abstract class Employee {
    abstract double calculatePay();
}

class HourlyEmployee extends Employee {
    private int hoursWorked;
    private double ratePerHour;

    HourlyEmployee(int hoursWorked, double ratePerHour) {
        this.hoursWorked = hoursWorked;
        this.ratePerHour = ratePerHour;
    }

    @Override
    double calculatePay() {
        return hoursWorked * ratePerHour;
    }
}

class SalariedEmployee extends Employee {
    private double monthlySalary;

    SalariedEmployee(double monthlySalary) {
        this.monthlySalary = monthlySalary;
    }

    @Override
    double calculatePay() {
        return monthlySalary;
    }
}

public class EmployeePayCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice = sc.nextInt();
        Employee emp;
        if (choice == 1) {
            int hours = sc.nextInt();
            double rate = sc.nextDouble();
            emp = new HourlyEmployee(hours, rate);
        } else if (choice == 2) {
            double salary = sc.nextDouble();
            emp = new SalariedEmployee(salary);
        } else {
            System.out.println("Invalid choice");
            sc.close();
            return;
        }
        System.out.printf("%.2f%n", emp.calculatePay());
        sc.close();
    }
}

```




## OUTPUT:

<img width="829" height="293" alt="image" src="https://github.com/user-attachments/assets/84226c00-0cfc-4bb3-a4dc-06bee17c174f" />


## RESULT:
Thus, the Java program implementing Abstraction using abstract classes and subclass-specific pay calculation was executed successfully.

