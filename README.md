# Java-program-for-comparison-of-two-numbers

## AIM:
To write a java program to compare two numbers and print the output.

## PROCEDURE:
1. Import the Scanner class from the java.util package to allow user input.
2. Define the class "Comparison" and the main method of the class.
3. Create a new Scanner object named "sc" to read input from the user.
4. Read the first integer and second integer input from the user and store it in a variable named "num1" and 'num2'.
5. Use an "if-else" statement to compare the values of "num1" and "num2".
6. Print the output according to the if-else statement conditions.
7. End the main method and the class definition.

## PROGRAM:
```
import java.util.Scanner;
public class Comparison{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter the numbers:");
        int num1 =sc.nextInt();
        int num2= sc.nextInt();
        if(num1==num2)
        {
            System.out.println("Both the numbers are equal.");
        }
        else if(num1>num2)
        {
            System.out.println(num1+" is greater than"+num2);
        }
        else
        {
            System.out.println(num2+" is greater than "+num1);
        }
    }
}
```
## OUTPUT:
```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=8098:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\Java 1\out\production\Java 1" Comparison
Enter the numbers:
10 45
45 is greater than 10

Process finished with exit code 0

```

## RESULT:
Thus the java program to compare two numbers is executed and the output is verified.







