# JAVA PROGRAMMING LANGUAGE
<br>

## What is Java
- Java is a popular programming language, created in 1995.
- Java is a portable language.

<br>

It is used for:
- Mobile applications (specially Android apps)
- Desktop applications
- Web applications
- Web servers and application servers
- Games
- Database connection
<br>

## BOILERPLATE CODE
<br>

- Boilerplate code or boilerplate refers to sections of code that have to be included in many places with little or no alteration.
- A boilerplate code usually refers to a pile of code blocks with a fixed pattern that can be widely applied to various program modules.
<br>

## Java Syntax
```
public class JavaBasics {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```
>OUTPUT : Hello World!

# PROGRAM QUESTIONS
## VARIABLES & DATA TYPES QUESTIONS
<br>

### Question1:
**In a program, input 3 numbers: A, B and C. You have to output the average of these 3 numbers. <br>(Hint : Average of N numbers is sum of those numbers divided by N)<br>**
**Program:**
```
import java.util.*;

public class JavaBasics{
    public static void main(String args[]){
        Scanner s = new Scanner(System.in);
        System.out.println("Input first no. :");
        float a = s.nextFloat();
        System.out.println("Input second no. :");
        float b = s.nextFloat();
        System.out.println("Input third no. :");
        float c = s.nextFloat();
        float avg = (a+b+c)/3 ;
        System.out.println("The average is :"+avg);
        s.close();
    }
}
```
>OUTPUT:
><br>
>Input first no. :
><br>
>2
><br>
>Input second no. :
><br>
>3
><br>
>Input third no. :
><br>
>6
><br>
>The average is :3.6666667
---

### Question2:
**In a program, input the side of a square. You have to output the area of the square.<br>(Hint : area of a square is (side x side)) <br>**
**Program**
```
import java.util.*;

public class JavaBasics{
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        System.out.print("Enter side of a square: ");
        float side = s.nextFloat();
        float area = side*side;
        System.out.println("The area of a square with side "+side+" is "+area);
        s.close();
    }
}
```
>OUTPUT:
><br>
>Enter side of a square: 6.5
><br>
>The area of a square with side 6.5 is 42.25
---

### Question3: 
**Enter cost of 3 items from the user (using float data type) - a pencil, a pen and an eraser. You have to output the total cost of the items back to the user as their bill. <br> (Add on : You can also try adding 18% gst tax to the items in the bill as an advanced problem) <br>**
**Program**
```
import java.util.*;
public class JavaBasics{
    public static void main(String[] args) {
       Scanner s = new Scanner(System.in);
       System.out.print("Enter price of a pencil : ");
       float mrp_pencil = s.nextFloat();
       System.out.print("Enter price of a pen :");
       float mrp_pen = s.nextFloat();
       System.out.print("Enter price of an eraser : ");
       float mrp_eraser = s.nextFloat();
       float total_cost = mrp_pencil+mrp_pen+mrp_eraser;
       System.out.println("The total cost of a pencil , a pen and an eraser is "+total_cost);

       //Add on - with 18% tax
       float newTotal=total_cost+ (0.18f*total_cost);
       System.out.println("Bill with 18% tax : "+newTotal);
       s.close();
    }
}
```
>OUTPUT:
><br>
>Enter price of a pencil : 5
><br>
>Enter price of a pen :10
><br>
>Enter price of an eraser : 5
><br>
>The total cost of a pencil , a pen and an eraser is 20.0
><br>
>Bill with 18% tax : 23.6
---

### Question 4:
**What will be the type of result in the following Java code?** <br>
![Ques1](https://github.com/Raveena-29/Java/assets/148243757/5f11dd17-e059-4f0c-980f-a3ea310efe0a)
<br>
**(Hint : Look at the largest data type among these)<br>**
**Solution**
<br>
In the mentioned code, the result variable will be of double type because oftype conversion.
--- 

### Question 5: 
**Will the following statement give any error in Java?**
```
int int$=24;
```
**Solution**<br>
No, the statement will not give any error.Names of variables are called identifiers in Java. Identifier rule says, identifier scan start with any alphabet or underscore (“_”) or dollar (“$”). According to the rule the given variable name is a valid identifier.
