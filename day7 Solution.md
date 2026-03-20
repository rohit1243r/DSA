# 🚀 Day 4 DSA Challenge (Java)

This repository contains solutions for **Day 7 of the DSA Challenge** using **Java**.
The programs focus on **Switch Case Statemnet**.

---

# 📌 Programs

---

# 1️⃣ Find the Smallest Number

```java
public static int smallestNo(int[] arr){
    int min = arr[0];
    for(int i=1; i<arr.length; i++){
        if(arr[i] < min) min = arr[i];
    }
    return min;
}
```

---

# 2️⃣ Find the Largest Number

```java
public static int smallestNo(int[] arr){
    int max = arr[0];
    for(int i=1; i<arr.length; i++){
        if(arr[i] > max) max = arr[i];
    }
    return max;
}
```

---

# 3️⃣ Second Smallest and Second Largest

```java
public static void secMinMax(int[] arr) {
    Arrays.sort(arr);
    System.out.println("Second Minimum: "+arr[1]);
    System.out.println("Second Maximum: "+arr[(arr.length)-2]);
}
```

---

# 4️⃣ Reverse a Given Array

```java
public static int[] revArray(int[] arr) {
        if(arr == null){
            return null;
        }
        int l = 0, r = arr.length-1;
        while(l < r){
            int temp = arr[l];
            arr[l] = arr[r];
            arr[r] = temp;
            l++;
            r--;
        }
        return arr;
    }
```   

---

# 5️⃣ Count Frequency of Each Element

```java
public static void freqEachElem(int[] arr) {
        if(arr == null){
            System.out.println(-1);
            return;
        }
        HashMap<Integer, Integer> map = new HashMap<>();
        for(int num : arr){
            map.put(num , map.getOrDefault(num, 0)+1);
        }
        for(Map.Entry<Integer, Integer> entry : map.entrySet()) {
            System.out.println(entry.getKey()+" "+entry.getValue());
        }
        
    }
```

---

# 6️⃣ Rearrange in Increasing-Decreasing Order

```java
public static void inDeOrder(int[] arr) {
        if(arr == null || arr.length == 0){
            return;
        }
        Arrays.sort(arr);
        int n = arr.length;
        int mid = (n + 1) / 2;
        int l = mid, r = n-1;
        while(l < r){
            int temp = arr[l];
            arr[l] = arr[r];
            arr[r] = temp;
            l++;
            r--;
        }
    }
```    

---

# 7️⃣ Sum of All Elements

```java
public static int sumOfElemet(int[] arr) {
        if(arr == null || arr.length == 0){
            return -1;
        }
        int sum = 0;
        for(int n : arr){
            sum += n;
        }
        return sum;
    }
```

---

# 8️⃣ Average of All Elements

```java
public static double avgOfAllElm(int[] arr) {
        if(arr == null || arr.length == 0){
            return -1;
        }
        int sum = 0;
        for(int n : arr){
            sum += n;
        }
        return (double) sum / arr.length;
    }
```

---

# 9️⃣ Median of the Array

```java
public static double medianArray(int[] arr) {
        if(arr == null || arr.length == 0){
            return -1;
        }
        Arrays.sort(arr);
        int n = arr.length;
        if(n % 2 == 0){
            return (arr[n/2-1] + arr[n/2]) / 2.0;
        }
        return arr[n/2];
    }
```

---

# 🎯 Challenge

This repository is part of my **60-70 Days of Java / DSA Challenge** where I solve coding problems daily to improve my **problem-solving and programming skills**.

⭐ If you like this repository, consider **starring it!**