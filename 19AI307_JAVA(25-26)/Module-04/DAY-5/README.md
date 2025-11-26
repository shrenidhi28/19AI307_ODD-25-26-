# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION: Design a program where a Product model stores item info, and the view displays it. Implement a controller to update product price and refresh the view automatically.




## AIM: To implement a **Behavioural Design Pattern (MVC pattern)** in Java where the **model** (Product) stores data, the **view** displays it, and the **controller** updates data and refreshes the view automatically.

---


## ALGORITHM

1. Start the program.  
2. Import the necessary package `java.util.Scanner`.  
3. Create a **Product class (Model)** to store `name`, `price`, and `code`. Include getter and setter methods.  
4. Create a **ProductView class (View)** with a method `displayProduct()` to display product details.  
5. Create a **ProductController class (Controller)** that:  
   - Accepts a Product and ProductView object.  
   - Provides a method `updateView()` to display the current product data.  
   - Provides a method `updatePrice(double newPrice)` to update the product price and refresh the view automatically.  
6. In the `main()` method:  
   - Accept user input for product `name`, `price`, `code`, and a `newPrice`.  
   - Create Product, ProductView, and ProductController objects.  
   - Call `updateView()` to display initial product details.  
   - Call `updatePrice(newPrice)` to update the price and refresh the view.  
7. Close the scanner and end the program.





## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: shrenidhi
RegisterNumber:
import java.util.Scanner;

public class ProductManagementSystem {

    // ===== Model =====
    static class Product {
        private String name;
        private double price;
        private String code;

        public Product(String name, double price, String code) {
            this.name = name;
            this.price = price;
            this.code = code;
        }

        public String getName() {
            return name;
        }

        public double getPrice() {
            return price;
        }

        public String getCode() {
            return code;
        }

        public void setPrice(double price) {
            this.price = price;
        }
    }

    // ===== View =====
    static class ProductView {
        public void displayProduct(String name, double price, String code) {
            System.out.println("--- Product Details ---");
            System.out.println("Name : " + name);
            System.out.println("Price: " + price);
            System.out.println("Code : " + code);
        }
    }

    // ===== Controller =====
    static class ProductController {
        private Product product;
        private ProductView view;

        public ProductController(Product product, ProductView view) {
            this.product = product;
            this.view = view;
        }

        public void updateView() {
            view.displayProduct(product.getName(), product.getPrice(), product.getCode());
        }

        public void updatePrice(double newPrice) {
            product.setPrice(newPrice);
            updateView();
        }
    }

    // ===== Main Method =====
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();
        double price = sc.nextDouble();
        sc.nextLine();
        String code = sc.nextLine();
        double newPrice = sc.nextDouble();

        Product product = new Product(name, price, code);
        ProductView view = new ProductView();
        ProductController controller = new ProductController(product, view);

        controller.updateView();
        controller.updatePrice(newPrice);

        sc.close();
    }
}

*/
```

## SOURCE CODE:

```
import java.util.Scanner;

public class ProductManagementSystem {

    // ===== Model =====
    static class Product {
        private String name;
        private double price;
        private String code;

        public Product(String name, double price, String code) {
            this.name = name;
            this.price = price;
            this.code = code;
        }

        public String getName() {
            return name;
        }

        public double getPrice() {
            return price;
        }

        public String getCode() {
            return code;
        }

        public void setPrice(double price) {
            this.price = price;
        }
    }

    // ===== View =====
    static class ProductView {
        public void displayProduct(String name, double price, String code) {
            System.out.println("--- Product Details ---");
            System.out.println("Name : " + name);
            System.out.println("Price: " + price);
            System.out.println("Code : " + code);
        }
    }

    // ===== Controller =====
    static class ProductController {
        private Product product;
        private ProductView view;

        public ProductController(Product product, ProductView view) {
            this.product = product;
            this.view = view;
        }

        public void updateView() {
            view.displayProduct(product.getName(), product.getPrice(), product.getCode());
        }

        public void updatePrice(double newPrice) {
            product.setPrice(newPrice);
            updateView();
        }
    }

    // ===== Main Method =====
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();
        double price = sc.nextDouble();
        sc.nextLine();
        String code = sc.nextLine();
        double newPrice = sc.nextDouble();

        Product product = new Product(name, price, code);
        ProductView view = new ProductView();
        ProductController controller = new ProductController(product, view);

        controller.updateView();
        controller.updatePrice(newPrice);

        sc.close();
    }
}

```






## OUTPUT:
<img width="961" height="363" alt="image" src="https://github.com/user-attachments/assets/41e23b9f-3afe-4a45-87e8-56809d1dd34b" />




## RESULT:
The program successfully demonstrates a Behavioural Design Pattern (MVC) in Java
