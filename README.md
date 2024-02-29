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

## OPERATORS IN JAVA

### TYPES OF OPERATORS
- Arithmatic operators (Binary , Unary, Ternary)
  - Binary : atleast 2 oprands
  - Unary : 1 oprand
    - Increment
      - Pre increment : ++a
      - Post increment : a++
    - Decrement
- Relational operators
- Logical operators
- Bitwise operators
- Assignment operators

### ARITHMETIC OPERATORS
|Binary|Unary|
|---|---|
|+ (Addition)|++ (Increment operator)|
|- (Subraction)|-- (Decrement operator)|
|* (Multiplication)||
|/ (Division)||
|% (Modulo)||





# PROGRAM QUESTIONS
## VARIABLES & DATA TYPES QUESTIONS
<br>

### Question 1:
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

### Question 2:
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

### Question 3: 
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

**What will be the type of result in the following Java code?** 
<br>

![Ques1](https://github.com/Raveena-29/Java/assets/148243757/5f11dd17-e059-4f0c-980f-a3ea310efe0a)

<br>

**(Hint : Look at the largest data type among these)** <br>

**Solution**  <br>
In the mentioned code, the result variable will be of double type because oftype conversion.

--- 

### Question 5: 
**Will the following statement give any error in Java?**
```
int int$=24;
```
**Solution**<br>
No, the statement will not give any error.Names of variables are called identifiers in Java. Identifier rule says, identifier scan start with any alphabet or underscore (“_”) or dollar (“$”). According to the rule the given variable name is a valid identifier.

### Question 6:
**Write a Java program to get a number from the user and print whether it is positive or negative.** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter any number : ");
        int num = sc.nextInt();
        sc.close();
        if(num>=0){
            System.out.println("Number is positive.");
        }
        else{
            System.out.println("Number is negative.");
        }
    }
}
```
>OUTPUT: <br>
>Enter any number : -8 <br>
>Number is negative.
---
###   Question 7:
**Finish the following code so that it prints "You have a fever" if your temperature is above 100 and otherwise prints "You don't have a fever".** <br>
```
public class JavaBasics{
    public static void main(String args[]){
        double temp=103.5;
    }
}
```
**Solution**
```
public class JavaBasics{
    public static void main(String args[]){
        double temp=103.5;
        if(temp>=100){
            System.out.print("You have a fever!");
        }
        else{
            System.out.println("You don't have a fever.");
        }
    }
}
```
>**OUTPUT :** <br>
>You have a fever!
---
### Question 8:
**Write a Java program to input week number(1-7) and print day of week name using switch case.**
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc= new Scanner(System.in);
        System.out.print("Enter week number (1-7) :");
        int day=sc.nextInt();
        sc.close();
        switch (day) {
            case 1:
                System.out.println("MONDAY");
                break;
            case 2:
                System.out.println("TUESDAY");
                break;
            case 3:
                System.out.println("WEDNESDAY");
                break;
            case 4:
                System.out.println("THURSDAY");
                break;
            case 5:
                System.out.println("FRIDAY");
                break;
            case 6:
                System.out.println("SATURDAY");
                break;
            case 7:
                System.out.println("SUNDAY");
                break;
            default:
                throw new AssertionError();
        }
    }
}
```
>**OUTPUT :** <br>
>Enter week number (1-7) :5 <br>
>FRIDAY
---
### Question 9:
**What will be the value of x & y in thefollowing program?** <BR>
```
public class JavaBasics{
    public static void main (String args[]){
        int a =63,b=36;
        boolean x= (a<b)?true:false;
        int y= (a>b)?a:b;
        System.out.println(x);
        System.out.println(y);
    }
}
```
**Solution :**  <br>
x -> False  <br>
y -> 63

---
### Question 10:
**Write a Java program that takes a year from the user and print whether that year is a leap year or not.** <br>
**Solution** <br>
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter a year : ");
        int year=sc.nextInt();
        boolean x= (year%4)==0;
        boolean y= (year%100)!=0;
        boolean z= (year%400)==0;
        if((x&&y)||z){
            System.out.println(year+" is a leap year.");
        }
        else{
            System.out.print(year+" is not a leap year.");
        }
    }
}
```
---
### Question 11:
**Print number from 1 to 10.** <br>
**Solution** <br> 
```
public class JavaBasics{
    public static void main(String args[]){
        int count=1;
        while(count<=10){
            System.out.println(count);
            count++;
        }
    }
}
```
---
### Question 12:
**Print number from 1 to nth (Take n through keyboard).** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        int count=1;
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter nth digit to print counting from 1 to n : ");
        int n =sc.nextInt();
        while(count<=n){
            System.out.println(count);
            count++;
        }
    }
}
```
---
### Question 13:
**Print sum of first n natural numbers.** <br>
**Solution**<br>
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        int count=1;
        int sum=0;
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter nth digit : ");
        int n =sc.nextInt();
        while(count<=n){
            sum+=count;
            count++;
        }
        System.out.println(sum);
    }
}
```
---
### Question 14:
**Print the given star pattern: <br> ****<br>****<br>****<br>****<br>** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of star in a side of the square pattern :");
        int n = sc.nextInt();
        for(int i=0;i<n;i++){
            for(int j=1;j<n;j++){
                System.out.print("*");
            }
        System.out.println("*");
        }
    }
}
```
### Question 15:
**Write a program to print n number in reverse order.** <br>
**Solution :**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc=  new Scanner(System.in);
        System.out.println("Enter any number : ");
        int n =sc.nextInt();
        System.out.println("The reverse of the number :");
        while(n>0){
            int remainder=n%10;
            System.out.print(remainder);
            n/=10;
        }
    
    }
}
```
>**OUTPUT :** <br>
>Enter any number :  <br>
>123 <br>
>The reverse of the number : <br>
>321
---
### Question 16:
**Write a program to print the reverse of a given number.**
```
public class JavaBasics{
    public static void main(String args[]){
        int num=1475902;
        int rev=0;
        while(num>0){
            int remainder=num%10;
            rev=(rev*10)+remainder;
            num/=10;
        }
    System.out.println("The reverse order of the number is "+rev);
    }
}
```
>**OUTPUT :** <br>
>The reverse order of the number is 2095741
---
### QUESTION 17: 
**Take a number as input from the user and keep printing it until the number is a multiple of 10.** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String[] args){
        Scanner sc =new Scanner(System.in);
        do{
            System.out.print("Enter any digit :");
            int num=sc.nextInt();
            if(num%10==0){
                break;
            }
            else{
                System.out.println(num);
            }
        }while(true);
        sc.close();
    }
}
```
---
### QUESTION 18:
**Take a number as input from the user and keep printing it.Skip the number if it is a multiple of 10.** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String[] args){
        Scanner sc =new Scanner(System.in);
        do{
            System.out.print("Enter any digit :");
            int num=sc.nextInt();
            if(num%10==0){
                continue;
            }
            else{
                System.out.println(num);
            }
        }while(true);
    }
}
```
---
### QUESTION 19:
**Check whether a number is prime or not** <br>
**Solution** 
```
import java.util.*;
public class JavaBasics{
    public static void main(String[] args){
        Scanner sc= new Scanner(System.in);
        System.out.print("Enter your number : ");
        int n=sc.nextInt();

        boolean isPrime=true;
        if(n==2){
            System.out.println(n+" is a prime number.");
        }
        else if(n==1){
            System.out.println(n+" is not a prime number.");
        }
        else{
            for (int i = 2; i <=Math.sqrt(n); i++) { 
                if(n%i==0){
                    isPrime=false;
                }
            }
        
            if(isPrime==true){
                System.out.println(n+" is a prime number");
            }
            else{
                System.out.println(n+" is not a prime number.");
            }
        }
    }
}
```
---
### QUESTION 20: 
**Write a program that reads a set of integers, and then prints the sum of the even and odd integers.** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter the no. of integer element in your set:");
        int n =sc.nextInt();
        int even=0;
        int odd=0;


        for (int i=1;i<=n;i++){
            System.out.println("Enter the number:");
            int integers=sc.nextInt();
            System.out.println("Your number is :"+integers);
            if (integers%2==0){
                even+=integers;
            }
            else{
                odd+=integers;
            }
        }
        System.out.println("The sum of even integers: "+even);
        System.out.println("The sum of odd integers: "+odd);
    }
}
```
---
### QUESTION 21
**Write a program to find the factorialof any number entered by the user.** <br>
**Solution:**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String[]args) {
        Scanner sc=new Scanner(System.in);
        int num;// To hold number
        int fact=1;// To hold factorial
        System.out.print("Enter any positive integer:");
        num=sc.nextInt();   
        for(int i=1;i<=num;i++) {  
            fact*=i; 
        }
        System.out.println("Factorial: "+fact);
    }
}
```
---
### QUESTION 22
**Write a program to print the multiplication table of a number N, entered by the user.** <br>
**Solution:**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your number: ");
        int num = sc.nextInt();
        for (int i=1;i<=10;i++){
            int multi=num*i;
            System.out.println(num+" X "+i+" = "+multi);
        }
    }
}
```
### QUESTION 23
**Print inverted star pattern.** <br>
**Solution**
```
import java.util.Scanner;
public class JavaBasics{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        int num=sc.nextInt();
        for(int i=0;i<num;i++){
            for(int j=1;j<num-i+1;j++){
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```
