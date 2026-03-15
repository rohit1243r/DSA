# 🚀 Day 2 – DSA Challenge (Java)

This repository contains solutions for **Day 2 of the DSA Challenge** using **Java**.
The programs focus on **basic Java concepts like input, conditions, loops, and strings**.

---

# 📌 Programs

---

# 1️⃣ Even or Odd Number

```java
import java.util.Scanner;

public class EvenOdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        if(n % 2 == 0){
            System.out.println("Even");
        }else{
            System.out.println("Odd");
        }

        sc.close();
    }
}
```

---

# 2️⃣ Greeting Message

```java
import java.util.Scanner;

public class Greeting {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();

        System.out.println("Hello " + name + ", welcome to the DSA Challenge!");

        sc.close();
    }
}
```

---

# 3️⃣ Simple Interest

Formula:

SI = (P × T × R) / 100

```java
import java.util.Scanner;

public class SimpleInterest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int P = sc.nextInt();
        int T = sc.nextInt();
        int R = sc.nextInt();

        double SI = (P * T * R) / 100.0;

        System.out.println("Simple Interest = " + SI);

        sc.close();
    }
}
```

---

# 4️⃣ Simple Calculator

```java
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        char operator = sc.next().charAt(0);
        int b = sc.nextInt();

        if(operator == '+'){
            System.out.println(a + b);
        }
        else if(operator == '-'){
            System.out.println(a - b);
        }
        else if(operator == '*'){
            System.out.println(a * b);
        }
        else if(operator == '/'){
            System.out.println(a / b);
        }

        sc.close();
    }
}
```

---

# 5️⃣ Largest of Two Numbers

```java
import java.util.Scanner;

public class LargestNumber {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        if(a > b){
            System.out.println(a);
        }
        else if(b > a){
            System.out.println(b);
        }
        else{
            System.out.println("Equal");
        }

        sc.close();
    }
}
```

---

# 6️⃣ INR to USD Converter

Conversion Rate:

1 USD = 83.5 INR

```java
import java.util.Scanner;

public class CurrencyConverter {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        double inr = sc.nextDouble();

        double usd = inr / 83.5;

        System.out.println("USD = " + usd);

        sc.close();
    }
}
```

---

# 7️⃣ Fibonacci Series

Example Output:
0 1 1 2 3 5 8

```java
import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        int a = 0;
        int b = 1;

        for(int i=0; i<n; i++){
            System.out.print(a + " ");

            int next = a + b;
            a = b;
            b = next;
        }

        sc.close();
    }
}
```

---

# 8️⃣ Palindrome String

```java
import java.util.Scanner;

public class Palindrome {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        String str = sc.nextLine();

        int i = 0;
        int j = str.length() - 1;

        boolean isPalindrome = true;

        while(i < j){
            if(str.charAt(i) != str.charAt(j)){
                isPalindrome = false;
                break;
            }

            i++;
            j--;
        }

        if(isPalindrome){
            System.out.println("Palindrome");
        }else{
            System.out.println("Not Palindrome");
        }

        sc.close();
    }
}
```

---

# 9️⃣ Armstrong Numbers in a Range

Example:
153 = 1³ + 5³ + 3³

```java
import java.util.Scanner;

public class ArmstrongRange {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int start = sc.nextInt();
        int end = sc.nextInt();

        for(int num = start; num <= end; num++){

            int temp = num;
            int sum = 0;

            while(temp > 0){
                int digit = temp % 10;

                sum += digit * digit * digit;

                temp /= 10;
            }

            if(sum == num){
                System.out.print(num + " ");
            }
        }

        sc.close();
    }
}
```

---

# 🛠 Technologies Used

* Java
* Scanner Class
* Loops
* Conditional Statements
* String Manipulation

---

# 🎯 Challenge

This repository is part of my **60-70 Days of Java / DSA Challenge** where I solve coding problems daily to improve my **problem-solving and programming skills**.

⭐ If you like this repository, consider **starring it!**
