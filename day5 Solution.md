# 🚀 Day 4 DSA Challenge (Java)

This repository contains solutions for **Day 4 of the DSA Challenge** using **Java**.
The programs focus on **Switch Case Statemnet**.

---

# 📌 Programs

---

# 1️⃣ .Find if a number is palindrome or not.

```java
import java.util.Scanner;
public class Solution{
   static boolean isPalindrome(int n){
        if(n < 0) return false;
        int temp = n;
        int x = 0;
        while(temp > 0) {
            int digit  = temp % 10;
            x = x * 10 + digit;
            temp /= 10;
        }
       return x==n;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n =sc.nextInt();
        boolean x = isPalindrome(n);
        System.out.println(x);
        sc.close(); 

    }
}
```

---

# 2️⃣ HCF and LCM of two numbers

```java
import java.util.Scanner;

public class Solution {
    static int hcf(int a, int b) {
        while(b != 0){
            int temp = b;
            b = a % b;
            a = temp;
        }
        return a;
    }
    static int lcm(int a, int b){
        return (a * b) / hcf(a, b);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();

        int h = hcf(a, b);
        int l = lcm(a, b);

        System.out.println("HCF: "+h);
        System.out.println("LCM: "+l);

        sc.close();
    }
}
```

---

# 3️⃣ Vowel or Consonant

```java
import java.util.Scanner;

public class Solution {
    static void Check(char ch){
        if(!Character.isLetter(ch)){
            System.out.println("Please Enter a Character");
            return;
        }
        ch = Character.toLowerCase(ch);
        if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u'){
            System.out.println("Vowel");
        }else{
            System.out.println("Consonent");
        }
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        char ch = in.next().charAt(0);
        Check(ch);
        in.close();
    }
}
```

---

# 4️⃣ Perfect Number

```java
import java.util.Scanner;

public class Solution {
    static boolean perfectNum(int n){
        if(n <= 1) return false;
        int sum = 0;
        for(int i=1; i <= n/2; i++){
            if(n % i == 0){
                sum += i;
            }
        }
        return sum == n;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        boolean p = perfectNum(n);
        System.out.println(p);
        in.close();
    }
}
```

---

# 5️⃣ Check Leap Year

```java
import java.util.Scanner;

public class Solution {
    static boolean leapYear(int n){
        return (n%4==0) && (n % 400 != 0 || n % 100 == 0);
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int year = in.nextInt();
        boolean p = leapYear(year);
        System.out.println(p);
        in.close();
    }
}
```

---

# 6️⃣ Sum of Digits of a Number

```java
import java.util.Scanner;

public class Solution {
    static int sumOfDigit(int n){
        int sum = 0;
        while(n > 0){
            int d = n % 10;
            sum += d;
            n /= 10;
        }
        return sum;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int year = in.nextInt();
        int x = sumOfDigit(year);
        System.out.println(x);
        in.close();
    }
}
```

---

# 7️⃣ Kunal's Even Days (August)

```java
import java.util.Scanner;

public class Solution {
    static int count(int n){
        return n / 2;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int n = 31;
        int count = count(n);
        System.out.println(count);
        in.close();
    }
}
```

---

# 8️⃣ Sum of negative numbers, sum of positive even numbers, and sum of positive odd numbers from a list

```java
import java.util.Scanner;

public class Solution {
    public static void sumOfList() {
        int son = 0, sope = 0, sopo = 0;
        Scanner in = new Scanner(System.in);
        while (true) {
            int n = in.nextInt();
            if(n == 0){
                break;
            }
            if (n < 0) {
                son += n;
            }else if(n % 2 == 0){
                sope += n;
            }else{
                sopo += n;
            }
        }
        System.out.println("Sum of negative number : "+son);
        System.out.println("Sum of positive even number : "+sope);
        System.out.println("Sum of positive odd number : "+sopo);
        in.close();
    }
    public static void main(String[] args) {
        sumOfList();        
    }
}
```

---

# 9️⃣ Define two methods to print the maximum and minimum among three numbers entered by the user

```java
import java.util.Scanner;

public class Solution {
    public static int max(int a, int b, int c) {
        int max = Integer.MIN_VALUE;
        if(a > max){
            max = a;
        }
        if(b > max) {
            max = b;
        }
        if(c > max){
            max = c;
        }
        return max;
    }
    public static int min(int a, int b, int c){
        int min = Integer.MAX_VALUE;
        if(a < min){
            min = a;
        }
        if(b < min){
            min = b;
        }
        if(c < min){
            min = c;
        }
        return min;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int a = in.nextInt();
        int b = in.nextInt();
        int c = in.nextInt();   
        int max = max(a, b, c);
        int min = min(a, b, c);     
        System.out.println("Maximum : "+max);
        System.out.println("Minimum: "+min);
        in.close();
    }
}
```

---

# 🔟 Define a method to find whether a given number is even or odd

```java
import java.util.Scanner;

public class Solution {
    public static boolean oddEven(int a) {
        return a % 2 == 0;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int a = in.nextInt();
        boolean check = oddEven(a);
        if(check){
           System.out.println("Even"); 
        }else{
            System.out.println("Odd");
        }
        in.close();
    }
}
```

---

# 1️⃣1️⃣ Voting Eligibility

```java
import java.util.Scanner;

public class Solution {
    public static boolean votingEligibility(int age) {
        return age >= 18;
    }
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int age = in.nextInt();
        boolean check = votingEligibility(age);
        System.out.println(check);
        in.close();
    }
}
```

---

# 1️⃣2️⃣ Write a method that takes two numbers as input and returns their sum

```java
import java.util.Scanner;

public class Solution {
    public static int sum() {
        Scanner in = new Scanner(System.in);
        int a = in.nextInt();
        int b = in.nextInt();
        in.close();
        return a+b;        
    }
    public static void main(String[] args) {
        int sum = sum();
        System.out.println(sum);
    }
}
```

---

# 1️⃣3️⃣  Sum of N numbers entered by the user — list terminates when user enters 0

```java
import java.util.Scanner;

public class Solution {
    public static int sum() {
        Scanner in = new Scanner(System.in);
        int sum = 0;
        while(true){
            int n = in.nextInt();
            if(n == 0){
                break;
            }
            sum+=n;
        }
        in.close();
        return sum;        
    }
    public static void main(String[] args) {
        int sum = sum();
        System.out.println(sum);
    }
}
```

---

# 🎯 Challenge

This repository is part of my **60-70 Days of Java / DSA Challenge** where I solve coding problems daily to improve my **problem-solving and programming skills**.

⭐ If you like this repository, consider **starring it!**