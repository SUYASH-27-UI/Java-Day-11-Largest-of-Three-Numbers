# Java-Day-11-Largest-of-Three-Numbers
# Java Day 11 - Largest of Three Numbers

This program takes three numbers from the user and finds the largest number using conditional statements.

## Example

Input:

```text
25
42
18
```

Output:

```text
Largest number = 42
```

## Concepts Used

* Scanner
* User input
* Variables
* `if`
* `else if`
* `else`
* Comparison operators
* `&&` AND operator

## How It Works

1. The program creates a `Scanner` object.
2. The user enters three numbers.
3. The program compares the first number with the other two numbers.
4. If the first number is not the largest, the second number is checked.
5. If neither the first nor second number is largest, the third number is the largest.
6. The largest number is displayed.

## Java Code

```java
import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int num1 = sc.nextInt();

        System.out.print("Enter second number: ");
        int num2 = sc.nextInt();

        System.out.print("Enter third number: ");
        int num3 = sc.nextInt();

        if (num1 >= num2 && num1 >= num3)
        {
            System.out.println("Largest number = " + num1);
        }
        else if (num2 >= num1 && num2 >= num3)
        {
            System.out.println("Largest number = " + num2);
        }
        else
        {
            System.out.println("Largest number = " + num3);
        }

        sc.close();
    }
}
```

## Output

```text
Enter first number: 25
Enter second number: 42
Enter third number: 18
Largest number = 42
```

## Goal

The goal of this project is to practice conditional statements, comparison operators, and the `&&` operator in Java.
