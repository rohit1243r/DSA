# 🚀 Day 4 DSA Challenge (Java)

This repository contains solutions for **Day 4 of the DSA Challenge** using **Java**.
The programs focus on **Switch Case Statemnet**.

---

# 📌 Programs

---

# 1️⃣ Is a Number Prime?

```java
import java.util.Scanner;

public class Solution {
    static boolean isPrime(int n){
        if(n <= 1) return false;
        if(n == 2) return true;
        if(n % 2 == 0) return false;
        for(int i=3; i<=Math.sqrt(n); i += 2){
            if(n % i == 0) return false;
        }
        return true;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        boolean x = isPrime(n);
        System.out.println(x);
        sc.close();
    }
}
```

---

# 2️⃣ Grade Calculator

```java
import java.util.Scanner;

public class Solution {
    static String getGrade(int n){
        String grade = "";
        if(n >= 91) grade = "AA";
        else if(n >= 81) grade = "AB";
        else if(n >= 71) grade = "BB";
        else if(n >= 61) grade = "BC";
        else if(n >= 51) grade = "CD";
        else if(n >= 41) grade = "DD";
        else grade = "Fail";
        return grade;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        String grade = getGrade(n);
        System.out.println(grade);
        sc.close();
    }
}
```

---

# 3️⃣ Factorial

```java
import java.util.Scanner;

public class Solution {
    static int factorial(int n){
        if(n == 0 || n == 1) return 1;
        int res = 1;
        for(int i = 2; i <= n; i++) res *= i;
        return res;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int fact = factorial(n);
        System.out.println(fact);
        sc.close();
    }
}
```

---

# 4️⃣ Palindrome Number

```java
import java.util.Scanner;

public class Solution {
    static boolean Palindrom(int n){
        if(n < 0) return false;
        int temp = n, rev = 0;
        while(temp > 0){
            int d = temp % 10;
            rev = rev * 10 + d;
            temp /= 10;
        }
        return n == rev;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        boolean res = Palindrom(n);
        System.out.println(res);
        sc.close();
    }
}
```

---

# 5️⃣ Refactor Previous Programs into Functions

```java
// isEven(int n) — from Day 2
import java.util.Scanner;

public class Solution {
    static boolean isEven(int n){
        return n % 2 == 0;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        boolean res = isEven(n);
        System.out.println(res);
        sc.close();
    }
}


// isLeapYear(int year) — from Day 2
import java.util.Scanner;

public class Solution {
    static boolean isLeapYear(int year){
        return (year % 4 == 0) && (year % 400 != 0 || year % 100 != 0);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int year = sc.nextInt();
        boolean res = isLeapYear(year);
        System.out.println(res);
        sc.close();
    }
}

// areaOfCircle(double r) — from Day 3

import java.util.Scanner;

public class Solution {
    static double areaOfTheCircule(int r){
        double aoc = 3.14*r*r;
        return aoc;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int r = sc.nextInt();
        double res = areaOfTheCircule(r);
        System.out.println(res);
        sc.close();
    }
}

//simpleInterest(double p, double t, double r) — from Day 2

import java.util.Scanner;

public class Solution {
    static double SimpleIntrest(int p , int r, int t){
        double si = (p * r * t) / 100;
        return si;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int p = sc.nextInt();
        int r = sc.nextInt();
        int t = sc.nextInt();

        double res = SimpleIntrest(p,r,t);
        System.out.println(res);
        sc.close();
    }
}

// fibonacci(int n) — from Day 3
import java.util.Scanner;
public class Solution {
    static void fibonacci(int n){
        int p = 0, q = 1;
        while(n > 0){
            System.out.println(p);
            int next = p + q;
            p = q;
            q = next;
            n--;
        }
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int p = sc.nextInt();
        fibonacci(p);
        sc.close();
    }
}
```

---

# 6️⃣ Pythagorean Triplet

```java
import java.util.Scanner;

public class Solution {
    static boolean isPythagorean(int a, int b, int c) {
        int nums[] = { a, b, c };
        java.util.Arrays.sort(nums);
        return nums[0] * nums[0] + nums[1] * nums[1] == nums[2] * nums[2];

    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();
        boolean rs = isPythagorean(a, b, c);
        System.out.println(rs);
        sc.close();
    }
}
```

---

# 7️⃣ All Primes Between Two Numbers

```java
import java.util.Scanner;

public class Solution {
    static boolean isPrime(int n){
        if(n <= 1) return false;
        if(n == 2) return true;
        if(n % 2 == 0) return false;
        for(int i=3; i <= Math.sqrt(n); i += 2){
            if(n % i == 0) return false;
        }
        return true;
    }
    static void primeNoBetweenTwoNo(int s, int e){
        for(int i = s; i <= e; i++){
            if(isPrime(i)){
                System.out.print(i+" ");
            }
        }
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int start = sc.nextInt();
        int end = sc.nextInt();
        primeNoBetweenTwoNo(start, end);
        sc.close();
    }
}
```

---

# 8️⃣ Sum of First N Natural Numbers

```java
import java.util.Scanner;

public class Solution {
    static long sumOfNNatural(int n){
        return (long) n * (n + 1) / 2;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        long sum = sumOfNNatural(n);
        System.out.println(sum);
        sc.close();
    }
}
```

---

# 🎯 Challenge

This repository is part of my **60-70 Days of Java / DSA Challenge** where I solve coding problems daily to improve my **problem-solving and programming skills**.

⭐ If you like this repository, consider **starring it!**