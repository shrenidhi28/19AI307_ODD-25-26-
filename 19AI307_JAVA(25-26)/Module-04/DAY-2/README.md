# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION: A city has sensors that measure Air Quality Index (AQI). There are three controllers that must monitor the AQI: GreenZoneController for AQI less than 100, AlertZoneController for AQI between 100 and 200, and DangerZoneController for AQI greater than 200. When a sensor reports its AQI value, only the controller responsible for that range should respond. Write a Java program using the Observer Pattern where SensorNetwork acts as the Subject and each controller acts as an Observer. Only the appropriate controller should react to each AQI reading.


## AIM:To implement the Observer design pattern in Java by creating a Sensor Network (Subject) and notifying only relevant SmartControllers (Observers) based on AQI conditions.


## Algorithm

1. Start the program.  
2. Import the necessary package: `java.util`.  
3. Define an **Observer interface** with a method `update(int aqi)`.  
4. Implement **concrete Observer classes**:  
   - `GreenZoneController` for AQI < 100.  
   - `AlertZoneController` for 100 ≤ AQI ≤ 200.  
   - `DangerZoneController` for AQI > 200.  
5. Define a **Subject interface** with methods:  
   - `registerObserver(Observer observer)` to add observers.  
   - `removeObserver(Observer observer)` to remove observers.  
   - `notifyObservers(int aqi)` to notify all observers.  
6. Implement **SensorNetwork** as a concrete Subject that maintains a list of observers.  
7. When a new AQI value is set, call `notifyObservers(aqi)`.  
8. Each Observer reacts only if the AQI falls in its designated range.  
9. In the `main()` method, create a `SensorNetwork` instance.  
10. Register all controllers (observers) with the SensorNetwork.  
11. Simulate AQI readings and display which controller reacts.  






## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: ShrenidhiC
RegisterNumber:212223040196
import java.util.*;

interface Observer {
    void check(int aqi, String sensorId);
}

class GreenZoneController implements Observer {
    //Type your code
    public void check(int aqi,String sensorId){
        if(aqi<100){
            
            System.out.println("[GreenZoneController]: AQI is good at Sensor " +sensorId + ". No action needed.");
        }
    }
}

class AlertZoneController implements Observer {
     //Type your code
     public void check(int aqi,String sensorId){
        if(aqi>=100 && aqi<=200){
            
            System.out.println("[AlertZoneController]: Moderate AQI at Sensor " + sensorId + ". Send public health alert.");
        }
    }
}

class DangerZoneController implements Observer {
     //Type your code
     public void check(int aqi,String sensorId){
        if(aqi>200){
           
            System.out.println("[DangerZoneController]: Critical AQI at Sensor "+ sensorId +"! Trigger lockdown protocol.");
        }
    }
}

class SensorNetwork {
     //Type your code
     List<Observer> observers = new ArrayList<>();
     void register(Observer obj){
         observers.add(obj);
     }
     void receiveData(String id, int aqi){
         System.out.println("Sensor " + id +" reports AQI: " + aqi);
         for(Observer o : observers){
             o.check(aqi,id);
         }
     }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        SensorNetwork network = new SensorNetwork();

        network.register(new GreenZoneController());
        network.register(new AlertZoneController());
        network.register(new DangerZoneController());

        int n = sc.nextInt(); sc.nextLine();
        for (int i = 0; i < n; i++) {
            String[] parts = sc.nextLine().split(" ");
            String id = parts[0];
            int aqi = Integer.parseInt(parts[1]);
            network.receiveData(id, aqi);
        }
    }
}

*/
```

## SOURCE CODE:

```
import java.util.*;

interface Observer {
    void check(int aqi, String sensorId);
}

class GreenZoneController implements Observer {
    //Type your code
    public void check(int aqi,String sensorId){
        if(aqi<100){
            
            System.out.println("[GreenZoneController]: AQI is good at Sensor " +sensorId + ". No action needed.");
        }
    }
}

class AlertZoneController implements Observer {
     //Type your code
     public void check(int aqi,String sensorId){
        if(aqi>=100 && aqi<=200){
            
            System.out.println("[AlertZoneController]: Moderate AQI at Sensor " + sensorId + ". Send public health alert.");
        }
    }
}

class DangerZoneController implements Observer {
     //Type your code
     public void check(int aqi,String sensorId){
        if(aqi>200){
           
            System.out.println("[DangerZoneController]: Critical AQI at Sensor "+ sensorId +"! Trigger lockdown protocol.");
        }
    }
}

class SensorNetwork {
     //Type your code
     List<Observer> observers = new ArrayList<>();
     void register(Observer obj){
         observers.add(obj);
     }
     void receiveData(String id, int aqi){
         System.out.println("Sensor " + id +" reports AQI: " + aqi);
         for(Observer o : observers){
             o.check(aqi,id);
         }
     }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        SensorNetwork network = new SensorNetwork();

        network.register(new GreenZoneController());
        network.register(new AlertZoneController());
        network.register(new DangerZoneController());

        int n = sc.nextInt(); sc.nextLine();
        for (int i = 0; i < n; i++) {
            String[] parts = sc.nextLine().split(" ");
            String id = parts[0];
            int aqi = Integer.parseInt(parts[1]);
            network.receiveData(id, aqi);
        }
    }
}

```







## OUTPUT:
<img width="961" height="276" alt="image" src="https://github.com/user-attachments/assets/46186eb9-6c7c-4668-bd4e-2700b15d0794" />



## RESULT:
The program successfully implements the Observer Pattern, notifying only the relevant controllers based on AQI values, demonstrating adherence to SOLID principles.

