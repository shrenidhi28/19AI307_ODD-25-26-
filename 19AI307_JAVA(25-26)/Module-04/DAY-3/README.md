# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION: Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).


## AIM:To implement Composition in Java by creating a Library class that contains multiple Book objects. The Book objects cannot exist independently outside the Library.


## ALGORITHM :


1. Start the program.  
2. Import the necessary package: `java.util.*`.  
3. Create a `Book` class with properties `title` and `author`, and a method `getDetails()` to return the book details.  
4. Create a `Library` class containing a `List<Book>` to store book objects.  
5. In the Library class, implement a method `addBook(String title, String author)` to create and add Book objects to the list.  
6. Implement a method `showBooks()` in Library to display all books in the library.  
7. In the `main()` method, create a `Library` instance.  
8. Accept user input for the number of books.  
9. For each book, accept `title` and `author` from the user.  
10. Add each book to the Library using `addBook()`.  
11. Call `showBooks()` to display all books in the library.  
	





## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: shrenidhi 
RegisterNumber: 212223040196
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books = new ArrayList<>();

    public void addBook(String title, String author) {
        Book book = new Book(title, author);
        books.add(book);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book book : books) {
            System.out.println("- " + book.getDetails());
        }
    }
}
 
*/
```

## SOURCE CODE:

```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books = new ArrayList<>();

    public void addBook(String title, String author) {
        Book book = new Book(title, author);
        books.add(book);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book book : books) {
            System.out.println("- " + book.getDetails());
        }
    }
}

```






## OUTPUT:
<img width="961" height="500" alt="image" src="https://github.com/user-attachments/assets/6f43216a-bb7f-4e64-ac4c-cc26fa63b047" />



## RESULT:
The program successfully demonstrates Composition in Java.
