# introduction to Java

here you will find the codes for everything we made in the course 


#### hello world 👋🏻

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```
#### variables 📝



```java
public class variables {
    public static void main(String[] args) {
        //int
    int myInt = 42;
        //string
    String myString = "Hello, world!";
        //double
    double myDouble = 3.14;
        //float
    long myLong = 123456789L;
        //boolean
    boolean myBoolean = true;
        //char
    char myChar = 'a';
        //byte
    byte myByte = 127;
        // print
        System.out.println("myInt = " + myInt);
        System.out.println("myString = " + myString);
        System.out.println("myDouble = " + myDouble);
        System.out.println("myLong = " + myLong);
        System.out.println("myBoolean = "+ myBoolean);
        System.out.println("myChar = " + myChar);
        System.out.println("myByte = " + myByte);

    }
}
```

#### operators 🧮

##### arithmetic operators

```java
public class operators {
    public static void main(String[] args) {
        int x = 5;
        int y = 3;

        // add
            int sum = x + y;
        // subtract
            int sub = x - y;
        // multiply
            int mul = x * y;
        // divide
            int div = x / y;
        // modulo
            int mod = x % y;
        // print
            System.out.println("sum = " + sum);
            System.out.println("sub = " + sub);
            System.out.println("mul = " + mul);
            System.out.println("div = " + div);
            System.out.println("mod = " + mod);
    }}
```

##### logical operators

```java
public class operators {
    public static void main(String[] args) {
        int x = 5;
        int y = 3;

        // and
            boolean and = x > 3 && y < 2;
        // or
            boolean or = x > 3 || y < 2;
        // not
            boolean not = !(x > 3 && y < 2);
        // print
            System.out.println("and = " + and);
            System.out.println("or = " + or);
            System.out.println("not = " + not);
    }}
```

##### relational operators

```java
public class operators {
    public static void main(String[] args) {
        int x = 5;
        int y = 3;

        // equal
            boolean equal = x == y;
        // not equal
            boolean notEqual = x != y;
        // greater than
            boolean greaterThan = x > y;
        // less than
            boolean lessThan = x < y;
        // greater than or equal
            boolean greaterThanOrEqual = x >= y;
        // less than or equal
            boolean lessThanOrEqual = x <= y;
        // print
            System.out.println("equal = " + equal);
            System.out.println("notEqual = " + notEqual);
            System.out.println("greaterThan = " + greaterThan);
            System.out.println("lessThan = " + lessThan);
            System.out.println("greaterThanOrEqual = " + greaterThanOrEqual);
            System.out.println("lessThanOrEqual = " + lessThanOrEqual);
    }}
```


#### Scanner 📠

```java
import java.util.Scanner;
public class scanner {
    public static void main(String[] args) {
        // create a scanner object
        Scanner scanner = new Scanner(System.in);
        // output the prompt
        System.out.println("Enter a line of text: ");
        // wait for the user to enter a line of text
        String line = scanner.nextLine();
        // tell them what they entered
        System.out.println("You entered: " + line);
    }
}
```


#### example1 📝

```java
import java.util.Scanner;
public class example {
    public static void main(String[] args) {
        // create a scanner object
        Scanner scanner = new Scanner(System.in);
        // output the prompt
        System.out.println("Enter the first number: ");
        // wait for the user to enter a number
        int number1 = scanner.nextInt();
        // output the prompt
        System.out.println("Enter the second number: ");
        // wait for the user to enter a number
        int number2 = scanner.nextInt();
        // add 
        System.out.println("The sum of " + number1 + " and " + number2 + " is " + (number1 + number2));
        // subtract
        System.out.println("The difference between " + number1 + " and " + number2 + " is " + (number1 - number2));
        // multiply
        System.out.println("The product of " + number1 + " and " + number2 + " is " + (number1 * number2));
        // divide
        System.out.println("The quotient of " + number1 + " and " + number2 + " is " + (number1 / number2));
    }
}
```

#### example2 📝

```java
import java.text.DecimalFormat;
import java.util.Locale;
import java.util.Scanner;
public class UserInfo {
    public static void main(String[] args) {
        Locale.setDefault(new Locale("es", "US"));
        Locale locale = Locale.getDefault();
		 Scanner scanner = new Scanner(System.in);
	        System.out.print("Enter your name: ");
	        String name = scanner.nextLine();
	        System.out.print("Enter your age: ");
	        int age = scanner.nextInt();
	        scanner.nextLine();
	        System.out.print("Enter your country: ");
	        String country = scanner.nextLine();
	        System.out.print("Enter your GPA: ");
	        double gpa = scanner.nextDouble();
	        scanner.nextLine();
	        System.out.print("Enter your gender: ");
	        String gender = scanner.nextLine();
	        System.out.println("Name: " + name);
	        System.out.println("Age: " + age);
	        System.out.println("Country: " + country);
	        System.out.println("GPA: " + gpa);
	        System.out.println("Gender: " + gender);
             }}
```

#### conditions 📝

##### If-else 1

```java
int x = 5;
int y = 10;
System.out.println("x = " + x + " y = " + y);
if (x > y) {
    System.out.println("x is greater than y");
} else if (x < y) {
    System.out.println("x is less than y");
} else {
    System.out.println("x is equal to y");
}
```

##### If-else 2

```java
int num1 = 10;
int num2 = 20;
int num3 = 30;
System.out.println("num1 = " + num1 + " num2 = " + num2 + " num3 = " + num3);

if (num1 > num2 && num1 > num3) {
    System.out.println(num1 + " is the largest number.");
} else if (num2 > num1 && num2 > num3) {
    System.out.println(num2 + " is the largest number.");
} else {
    System.out.println(num3 + " is the largest number.");
}
```

##### switch 1

```java
import java.util.Scanner;

public class DayName {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of the day (1-7): ");
        int dayNumber = scanner.nextInt();
       
        switch (dayNumber) {
            case 1:
               System.out.println("the day is Sunday");
                break;
            case 2:
                System.out.println("the day is Monday");
                break;
            case 3:
                System.out.println("the day is Tuesday");
                break;
            case 4:
                System.out.println("the day is Wednesday");
                break;
            case 5:
                System.out.println("the day is Thursday");
                break;
            case 6:
                System.out.println("the day is Friday");
                break;
            case 7:
                System.out.println("the day is Saturday");
                break;
            default:
                System.out.println("Invalid day number.");
 }}}
```
##### switch 2

```java
import java.util.Scanner;

public class Grade {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the grade: ");
        String grade = scanner.nextLine();
        grade = grade.toUpperCase();
        switch (grade) {
            case "A":
               System.out.println("Excellent!");
                break;
            case "B":
                System.out.println("Good!");
                break;
            case "C":
                System.out.println("Average!");
                break;
            case "D":
                System.out.println("Poor!");
                break;
            case "F":
                System.out.println("Fail!");
                break;
            default:
                System.out.println("Invalid grade.");
        
 }}}
```


#### loops 🔄

##### while loop

```java
import java.util.Scanner;

public class TextChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
    String expectedText = "Hello";
    String userInput = "";

    while (!userInput.equals(expectedText)) {
        System.out.print("Type the text: ");
        userInput = scanner.nextLine();

        if (!userInput.equals(expectedText)) {
            System.out.println("Incorrect text. Try again.");
        }
    }
    System.out.println("Correct text!");
    }
}
```


##### do-while loop

```java
import java.util.Scanner;

public class Menu {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
    int choice;

    do {
        System.out.println("Choose a number:");
        System.out.println("1. to Print 'Hello World'");
        System.out.println("2. to Print 'IEEE'");
        System.out.println("3. Exit");
        System.out.print("Enter your choice: ");
        choice = scanner.nextInt();

        switch (choice) {
            case 1:
                System.out.println("\nHello World\n");
                break;
            case 2:
                System.out.println("\nIEEE\n");
                break;
            case 3:
                System.out.println("\nExiting...\n");
                break;
            default:
                System.out.println("\nInvalid choice. Try again.\n");
                break;
        }
    } while (choice != 3);
    }
}

```

##### for loop

```java
import java.util.Scanner;

public class Factorial {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int num = scanner.nextInt();
        int factorial = 1;

        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }

        System.out.println("Factorial of " + num + " is " + factorial);
    }
}

```


#### methods 📝


##### int methods

```java
import java.util.Scanner;

public class Calc {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter first number: ");
        int num1 = scanner.nextInt();
        System.out.print("Enter second number: ");
        int num2 = scanner.nextInt();
        System.out.println("Sum = " + calcSum(num1, num2));
    }

    public static int calcSum(int num1, int num2) {
        return num1 + num2;
    }
   
}
```


##### void methods

```java
import java.util.Scanner;

public class Factorial {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int num = scanner.nextInt();
        getFactorial(num);
    }

    public static void getFactorial(int num) {
        int factorial = 1;

        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }

        System.out.println("Factorial of " + num + " is " + factorial);
    } 
}

```

#### arrays 📝

##### array 1

```java
import java.util.Random;

public class ArraySum {
    public static void main(String[] args) {
         int[] arr = {5,4,3,6,10};
      

      // calculate the sum of the array
      int sum = 0;
      for (int i = 0; i < arr.length; i++) {
          sum += arr[i];
      }
  
      System.out.println("the sum of the array : " + sum);
    }
}
```



## conclusion 📝

this is the end of the course, i hope you enjoyed it and learned something new, if you have any questions you can contact me on discord:  `@gogo.13` , `@yaj.13`  or you can make a pull request and i will answer you as soon as possible

thank you for your time and have a nice day

this course was made by: `yaj-13` for IEEE Taibah University Student Branch