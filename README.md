Java program for Calculator - to design calculator with arithmetic operators.
Java Program for Calculator - This program will read two integer numbers and calculate the arithmetic operators, in this example we used switch case and if else statement. User will enter a choice after entering two numbers and based on user choice program will return the result.

Calculator Example using Java Program
/*Java program for Calculator.*/
 
import java.util.*;
 
public class Calculator{
 
     public static void main(String []args){
         int a,b,choice;
         float result=0;
         /*scanner class object to read values*/
         Scanner buf=new Scanner(System.in);
          
         System.out.print("Enter first number: ");
         a=buf.nextInt();
         System.out.print("Enter second number: ");
         b=buf.nextInt();
          
         System.out.print("\n1: Addition.\n2: Subtraction.");
         System.out.print("\n3: Multiplication.\n4: Divide.");
         System.out.print("\n5: Remainder.\n6: Exit.");
          
         System.out.print("\nEnter your choice: ");
         choice=buf.nextInt();
          
         switch(choice)
         {
             case 1:
                 result=(a+b); break;
             case 2:
                 result=(a-b); break;
             case 3:
                 result=(a*b); break;
             case 4:
                 result=(float)((float)a/(float)b); break;
             case 5:
                 result=(a%b); break;
             default:
                 System.out.println("An Invalid Choice!!!\n");
         }
         if(choice>=1 && choice<=5)
            System.out.println("Result is: " + result);
          
     }
}
    
    First Run:
    me@linux:~$ javac Calculator.java 

    me@linux:~$ java Calculator 
    Enter first number: 10
    Enter second number: 20 

    1: Addition.
    2: Subtraction. 
    3: Multiplication.
    4: Divide.
    5: Remainder. 
    6: Exit.
    Enter your choice: 4
    Result is: 0.5

    Second Run:
    me@linux:~$ java Calculator 
    Enter first number: 10
    Enter second number: 7

    1: Addition.
    2: Subtraction. 
    3: Multiplication.
    4: Divide.
    5: Remainder. 
    6: Exit.
    Enter your choice: 5
    Result is: 3.0

