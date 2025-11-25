# Ex.No:3(D)    INTERFACE 

## QUESTION: You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.




## AIM: To implement interfaces in Java by creating weather-analysis bots that predict weather conditions based on temperature.


## ALGORITHM :
1. Start the program.
2. Import the package `java.util.Scanner`.
3. Create an interface `Bot` with the method `Predict()`.
4. Create the class `SunBot` implementing `Bot`.
5. Add a temperature field `n` in `SunBot`.
6. Implement `Predict()` in `SunBot` to return "HOT" if n > 30, otherwise "MODERATE".
7. Create the class `RainBot` implementing `Bot`.
8. Add a temperature field `n` in `RainBot`.
9. Implement `Predict()` in `RainBot` to return "COLD" if n < 20, otherwise "WARM".
10. In `main()`, create a Scanner to read temperature and bot type.
11. If bot type is 1, create a `SunBot` object and set temperature.
12. If bot type is 2, create a `RainBot` object and set temperature.
13. Call the `Predict()` method on the selected bot.
14. Print the prediction to the user.
15. End the program.






## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Shrenidhi
RegisterNumber: 212223040196
import java.util.*;
interface Bot{
    String Predict();
}
class SunBot implements Bot{
    int n;
    public String Predict(){
        if(this.n>30){
            return "HOT";
        }
        else{
            return "MODERATE";
        }
    }
}
class RainBot implements Bot{
    int n;
    public String Predict(){
        if(this.n<20){
            return "COLD";
        }
        else{
            return "WARM";
        }
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n,m;
        n= sc.nextInt();
        m= sc.nextInt();
        if(m==1){
            SunBot obj = new SunBot();
            obj.n= n;
            System.out.println(obj.Predict());
        }
        else{
            RainBot obj = new RainBot();
            obj.n= n;
            System.out.println(obj.Predict());
        }
    }
}

*/
```

## SOURCE CODE:

```
import java.util.*;
interface Bot{
    String Predict();
}
class SunBot implements Bot{
    int n;
    public String Predict(){
        if(this.n>30){
            return "HOT";
        }
        else{
            return "MODERATE";
        }
    }
}
class RainBot implements Bot{
    int n;
    public String Predict(){
        if(this.n<20){
            return "COLD";
        }
        else{
            return "WARM";
        }
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int n,m;
        n= sc.nextInt();
        m= sc.nextInt();
        if(m==1){
            SunBot obj = new SunBot();
            obj.n= n;
            System.out.println(obj.Predict());
        }
        else{
            RainBot obj = new RainBot();
            obj.n= n;
            System.out.println(obj.Predict());
        }
    }
}
```





## OUTPUT:
<img width="829" height="237" alt="image" src="https://github.com/user-attachments/assets/23dca6f3-913b-47c3-8424-515a40b5c126" />



## RESULT:
Thus, the Java program demonstrating Interface implementation with weather prediction bots was successfully executed.
