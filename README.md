# Java-program-for-comparison-of-two-numbers

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

OUTPUT:

C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=8098:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\Java 1\out\production\Java 1" Comparison
Enter the numbers:
10 45
45 is greater than 10

Process finished with exit code 0
