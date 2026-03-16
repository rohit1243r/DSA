# 🚀 Day 3 DSA Challenge (Java)

This repository contains solutions for **Day 3 of the DSA Challenge** using **Java**.
The programs focus on **Loops, Conditional Statements**.

---

# 📌 Programs

---

# 1️⃣ Area of Circle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double r = sc.nextDouble();
        double aoc = Math.PI * (r * r);
        System.out.println(aoc);
        sc.close();
    }
}
```

---

# 2️⃣ Area of Triangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double base = sc.nextDouble();
        double height = sc.nextDouble();
        double aot = 0.5 * base * height;
        System.out.println(aot);
        sc.close();
    }
}
```

---

# 3️⃣ Area of Rectangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double length = sc.nextDouble();
        double breadth = sc.nextDouble();
        double aor = length * breadth;
        System.out.println(aor);
        sc.close();
    }
}
```

---

# 4️⃣ Area of Isosceles Triangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double base = sc.nextDouble();
        double height = sc.nextDouble();
        double aoit = 0.5 * base * height;
        System.out.println(aoit);
        sc.close();
    }
}
```

---

# 5️⃣ Area of Parallelogram

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double base = sc.nextDouble();
        double height = sc.nextDouble();
        double aop = base * height;
        System.out.println(aop);
        sc.close();
    }
}
```

---

# 6️⃣ Area of Rhombus

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double d1 = sc.nextDouble();
        double d2 = sc.nextDouble();
        double areaOfRhombus = 0.5 * d1 * d2;
        System.out.println(areaOfRhombus);
        sc.close();
    }
}
```

---

# 7️⃣ Area of Equilateral Triangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double side = sc.nextDouble();
        double areaOfEquilateralTriangle = ((Math.sqrt(3)/4) * Math.pow(side, 2));
        System.out.println(areaOfEquilateralTriangle);
        sc.close();
    }
}
```

---

# 8️⃣ Perimeter of Circle (Circumference)

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double r = sc.nextDouble();
        double pi = 3.14;
        double perimeterOfCircle = 2 * pi * r;
        System.out.println(perimeterOfCircle);
        sc.close();
    }
}
```

---

# 9️⃣ Perimeter of Equilateral Triangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double side = sc.nextDouble();
        double perimeterOfEquilateralTriangle = 3 * side;
        System.out.println(perimeterOfEquilateralTriangle);
        sc.close();
    }
}
```

---

# 1️⃣0️⃣ Perimeter of Parallelogram

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b  = sc.nextInt();
        int perimeterOfParallelogram = 2 * (a + b);
        System.out.println(perimeterOfParallelogram);
        sc.close();
    }
}
```

---

# 🛠 Technologies Used

* Java
* Scanner Class

---

# 🎯 Challenge

This repository is part of my **60-70 Days of Java / DSA Challenge** where I solve coding problems daily to improve my **problem-solving and programming skills**.

⭐ If you like this repository, consider **starring it!**