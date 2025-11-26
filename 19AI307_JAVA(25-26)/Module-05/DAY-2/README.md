# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:


## AIM: To implement **Serialization and Deserialization in Java** by storing a list of Student objects into a file and retrieving them.

---


## ALGORITHM :
1. Start the program.  
2. Import the necessary packages: `java.io.*`, `java.util.*`.  
3. Create a `Student` class that implements `Serializable` with fields: `id`, `name`, and `marks`.  
4. Implement a `toString()` method in `Student` to display student details.  
5. Create methods:  
   - `serializeStudents(List<Student> students, String fileName)` to write the list of students to a file using `ObjectOutputStream`.  
   - `deserializeStudents(String fileName)` to read the list of students from a file using `ObjectInputStream`.  
6. In the `main()` method:  
   - Accept the number of students.  
   - Accept each student's `id`, `name`, and `marks`.  
   - Add each student to a `List<Student>`.  
   - Call `serializeStudents()` to save the list to a file.  
   - Call `deserializeStudents()` to read the list from the file.  
   - Display the deserialized student details.  
7. Close the Scanner and terminate the program.
	





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: shrenidhi C
RegisterNumber: 212223040196
import java.io.*;
import java.util.*;

// Student class must implement Serializable
class Student implements Serializable {
    private static final long serialVersionUID = 1L;

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    @Override
    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class StudentSerializationUserInput {

    // Serialize list of students
    public static void serializeStudents(List<Student> students, String fileName) {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream(fileName))) {
            oos.writeObject(students);
            System.out.println("Students serialized successfully into: " + fileName);
        } catch (IOException e) {
            System.out.println("Error during serialization: " + e.getMessage());
        }
    }

    // Deserialize list of students
    @SuppressWarnings("unchecked")
    public static List<Student> deserializeStudents(String fileName) {
        List<Student> students = null;
        try (ObjectInputStream ois = new ObjectInputStream(new FileInputStream(fileName))) {
            students = (List<Student>) ois.readObject();
            System.out.println("Students deserialized successfully from: " + fileName);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println("Error during deserialization: " + e.getMessage());
        }
        return students;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<Student> students = new ArrayList<>();

        //System.out.print("Enter number of students: ");
        int n = scanner.nextInt();
        scanner.nextLine(); // consume newline

        for (int i = 0; i < n; i++) {
            //System.out.println("Enter details for student " + (i + 1) + ":");
            //System.out.print("ID: ");
            int id = scanner.nextInt();
            scanner.nextLine(); // consume newline
            //System.out.print("Name: ");
            String name = scanner.nextLine();
            //System.out.print("Marks: ");
            double marks = scanner.nextDouble();
            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        // Serialize students
        serializeStudents(students, fileName);

        // Deserialize students
        List<Student> deserializedStudents = deserializeStudents(fileName);

        // Display deserialized data
        if (deserializedStudents != null) {
            System.out.println("\nDeserialized Students:");
            for (Student s : deserializedStudents) {
                System.out.println(s);
            }
        }

        scanner.close();
    }
}
 
*/
```

## SOURCE CODE:

```
import java.io.*;
import java.util.*;

// Student class must implement Serializable
class Student implements Serializable {
    private static final long serialVersionUID = 1L;

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    @Override
    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class StudentSerializationUserInput {

    // Serialize list of students
    public static void serializeStudents(List<Student> students, String fileName) {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream(fileName))) {
            oos.writeObject(students);
            System.out.println("Students serialized successfully into: " + fileName);
        } catch (IOException e) {
            System.out.println("Error during serialization: " + e.getMessage());
        }
    }

    // Deserialize list of students
    @SuppressWarnings("unchecked")
    public static List<Student> deserializeStudents(String fileName) {
        List<Student> students = null;
        try (ObjectInputStream ois = new ObjectInputStream(new FileInputStream(fileName))) {
            students = (List<Student>) ois.readObject();
            System.out.println("Students deserialized successfully from: " + fileName);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println("Error during deserialization: " + e.getMessage());
        }
        return students;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<Student> students = new ArrayList<>();

        //System.out.print("Enter number of students: ");
        int n = scanner.nextInt();
        scanner.nextLine(); // consume newline

        for (int i = 0; i < n; i++) {
            //System.out.println("Enter details for student " + (i + 1) + ":");
            //System.out.print("ID: ");
            int id = scanner.nextInt();
            scanner.nextLine(); // consume newline
            //System.out.print("Name: ");
            String name = scanner.nextLine();
            //System.out.print("Marks: ");
            double marks = scanner.nextDouble();
            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        // Serialize students
        serializeStudents(students, fileName);

        // Deserialize students
        List<Student> deserializedStudents = deserializeStudents(fileName);

        // Display deserialized data
        if (deserializedStudents != null) {
            System.out.println("\nDeserialized Students:");
            for (Student s : deserializedStudents) {
                System.out.println(s);
            }
        }

        scanner.close();
    }
}

```






## OUTPUT:

<img width="961" height="393" alt="image" src="https://github.com/user-attachments/assets/960043c0-a915-4151-8091-91fa2117d307" />


## RESULT: 
The program successfully demonstrates Serialization and Deserialization in Java

