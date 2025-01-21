# Operators-
import java.util.Scanner;

public class OperationsDemo {

public static void main(String[] args) {

Scanner scanner = new Scanner(System.in);

// Read input values

System.out.print("Enter the first number: ");

int num1 = scanner.nextInt();

System.out.print("Enter the second number: ");

int num2 = scanner.nextInt();

System.out.print("Enter the third number: ");

int num3 = scanner.nextInt();

// Arithmetic Operations

System.out.println("\n--- Arithmetic Operations ---");
System.out.println("Addition (num1 + num2): " + (num1 + num2));

System.out.println("Subtraction (num1 - num2): " + (num1 - num2));

System.out.println("Multiplication (num1 * num2): " + (num1 * num2));

System.out.println("Division (num1 / num2): " + (num2 != 0 ? (num1 / num2) : "Division by

zero error"));

System.out.println("Modulus (num1 % num2): " + (num2 != 0 ? (num1 % num2) : "Division

by zero error"));

// Relational Operations

System.out.println("\n--- Relational Operations ---");

System.out.printf("num1 > num2: %b, num1 < num2: %b, num1 == num2: %b%n",

num1 > num2, num1 < num2, num1 == num2);

System.out.printf("num1 != num3: %b, num2 >= num3: %b, num3 <= num1: %b%n",

num1 != num3, num2 >= num3, num3 <= num1);

// Logical Operations

System.out.println("\n--- Logical Operations ---");

System.out.println("(num1 > num2) && (num2 > num3): " + ((num1 > num2) && (num2 >

num3)));

System.out.println("(num1 > num2) || (num2 > num3): " + ((num1 > num2) || (num2 >

num3)));

System.out.println("!(num1 > num2): " + (!(num1 > num2)));

// Ternary Operator

System.out.println("\n--- Ternary Operator ---");

String largest = (num1 > num2) ? (num1 > num3 ? "num1 is the largest" : "num3 is the

largest")

: (num2 > num3 ? "num2 is the largest" : "num3 is the largest");

System.out.println("Largest number is: " + largest);

scanner.close();

}

}



OUTPUT:

Enter the first number: 12

Enter the second number: 4
Enter the third number: 7

Arithmetic Operations

Addition (num1 + num2): 16

Subtraction (num1 - num2): 8

Multiplication (num1 * num2): 48

Division (num1 / num2): 3

Modulus (num1 % num2): 0

Relational Operations

num1 > num2: true, num1 < num2: false, num1 == num2: false

num1 != num3: true, num2 >= num3: false, num3 <= num1: true

Logical Operations

(num1 > num2) && (num2 > num3): false

(num1 > num2) || (num2 > num3): true

!(num1 > num2): false

Ternary Operator

Largest number is: num1 is the largest
