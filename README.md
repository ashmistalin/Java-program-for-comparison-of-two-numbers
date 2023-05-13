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


# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required library packages.
2. Import the dataset to operate on.
3. Split the dataset into required segments.
4. Predict the required output.
5. Run the programm. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: ASHMI.S
RegisterNumber:  212221040021
*/
import pandas as pd
data = pd.read_csv("/content/spam.csv",encoding = 'latin-1')
data.head()
data.info()
data.isnull().sum()
x = data["v1"].values
y = data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size = 0.2,random_state = 0)
from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()    
x_train = cv.fit_transform(x_train)
x_test = cv.transform(x_test)
from sklearn.svm import SVC
svc = SVC()
svc.fit(x_train,y_train)
y_pred = svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
```

## Output:
## HEAD:
![GITHUB LOGO](s1.png)
## INFO:
![GITHUB LOGO](s2.png)
## ISNULL:
![GITHUB LOGO](s3.png)
## SVC PREDICT:
![GITHUB LOGO](s4.png)
## ACCURACY:
![GITHUB LOGO](s5.png)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.





