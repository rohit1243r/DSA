# 🚀 Day 4 DSA Challenge (Java)

This repository contains solutions for **Day 4 of the DSA Challenge** using **Java**.
The programs focus on **Switch Case Statemnet**.

---

# 📌 Programs

---

# 1️⃣ Perimeter of Rectangle

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double l = sc.nextDouble();
        double b = sc.nextDouble();
        double perimeterOfRectangle = 2 * (l * b);
        System.out.println(perimeterOfRectangle);
        sc.close();
    }
}
```

---

# 2️⃣ Perimeter of Squire

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double side = sc.nextDouble();
        double perimeterOfSquire = 4 * side;
        System.out.println(perimeterOfSquire);
        sc.close();
    }
}
```

---

# 3️⃣ Perimeter of Rhombus

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double side = sc.nextDouble();
        double perimeterOfRhombus = 4 * side;
        System.out.println(perimeterOfRhombus);
        sc.close();
    }
}
```

---

# 4️⃣ Volume of Prism

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double baseArea = sc.nextDouble();
        double height = sc.nextDouble();
        double volumeOfPrism = baseArea * height;
        System.out.println(volumeOfPrism);
        sc.close();
    }
}
```

# 5️⃣ Volume of Cylinder

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double r = sc.nextDouble();
        double h = sc.nextDouble();
        double pi = 3.14;
        double volumeOfCylinder = pi * (r * r) * h;
        System.out.println(volumeOfCylinder);
        sc.close();
    }
}
```

---

# 6️⃣ Volume of Sphere

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double r = sc.nextDouble();
        double volumeOfSphere = (4.0/3.0) * Math.PI * Math.pow(r, 3);
        System.out.println(volumeOfSphere);
        sc.close();
    }
}
```

---

# 7️⃣ Volume of Pyramid

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double baceArea = sc.nextDouble();
        double height = sc.nextDouble();
        double volumeOfPyramid = (1.0/3.0) * baceArea * height;
        System.out.println(volumeOfPyramid);
        sc.close();
    }
}
```

---

# 8️⃣ Curved Surface Area of Cylinder

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double r = sc.nextDouble();
        double h = sc.nextDouble();
        double curvedSurfaceAreaOfCylinder = 2 * Math.PI * r * h;
        System.out.println(curvedSurfaceAreaOfCylinder);
        sc.close();
    }
}
```

---

# 9️⃣ Total Surface Area of Cube

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double side = sc.nextDouble();
        double totalSurfaceAreaOfCube = 6 * Math.pow(side, 2);
        System.out.println(totalSurfaceAreaOfCube);
        sc.close();
    }
}
```

---

# 1️⃣0️⃣ Fibonacci Series up to n numbers

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int a = 0, b =1;
        int count = 0;
        while(count < n){
            System.out.print(a+" ");
            int next = a + b;
            a = b;
            b = next;
            count++;
        }
        sc.close();
    }
}
```

---

# 1️⃣1️⃣ Subtract the Product and Sum of Digits of an Integer

```java
import java.util.Scanner;

public class Solution{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int pod = 1;
        int sod = 0;
        while(n > 0){
            int digit = n % 10;
            pod *= digit;
            sod += digit;
            n /= 10;
        }
        System.out.println(pod - sod);
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