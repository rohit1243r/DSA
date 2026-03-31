# 🚀 Day 8 DSA Challenge (Java)

This repository contains solutions for **Day 8 of the DSA Challenge** using **Java**.
The programs focus on **Switch Case Statemnet**.

---

# 📌 Programs

---

# 1️⃣ Build Array from Permutation — LC # 1920 Easy

```java
class Solution {
    public int[] buildArray(int[] nums) {
        int n = nums.length;
        int[] ans= new int[n];
        for(int i=0; i<n; i++){
           ans[i] = nums[nums[i]];
        }
        return ans;
    }
}
```

---

# 2️⃣ Concatenation of Array — LC # 1929 Easy

```java
class Solution {
    public int[] getConcatenation(int[] nums) {
        int n = nums.length;
        int[] ans = new int[n*2];
        for(int i = 0; i<nums.length; i++){
            ans[i] = nums[i];
            ans[i+n] = nums[i];
        }
        return ans;
    }
}
```

---

# 3️⃣ Running Sum of 1D Array — LC # 1480 Easy

```java
class Solution {
    public int[] runningSum(int[] nums) {
        for(int i=1; i<nums.length; i++){
            nums[i] += nums[i-1];
        }
        return nums;
    }
}
```

---

# 4️⃣ Richest Customer Wealth — LC # 1672 Easy

```java
class Solution {
    public int maximumWealth(int[][] accounts) {
        int wealth = 0;
        for(int[] customer : accounts){
            int sum = 0;
            for(int money : customer){
                sum += money;
            }
            wealth = Math.max(wealth, sum);
        }
        return wealth;
    }
}
```

---

# 5️⃣ Shuffle the Array — LC # 1470 Easy

```java
class Solution {
    public int[] shuffle(int[] nums, int n) {
        int[] dup = new int[n * 2];
        int i = 0;
        int j = n;
        int k = 0;
        while (k < 2 * n) {
            if (k % 2 == 0) {
                dup[k] = nums[i++];
            } else {
                dup[k] = nums[j++];
            }
            k++;
        }
        return dup;
    }
}
```

---

# 6️⃣ Kids With the Greatest Number of Candies — LC # 1431 Easy

```java
class Solution {
    public List<Boolean> kidsWithCandies(int[] candies, int extraCandies) {
        ArrayList<Boolean> res = new ArrayList<>();
        int max = 0;
        for(int c : candies) {
            if(c > max){
                max = c;
            }
        }
        for(int c : candies) {
            if(max <= c+extraCandies){
                res.add(true);
            }else{
                res.add(false);
            }
        }
        return res;
    }
}
```

---

# 7️⃣ Number of Good Pairs — LC # 1512 Easy

```java
class Solution {
    public int numIdenticalPairs(int[] nums) {
        int count = 0;
          for(int i = 0; i<nums.length; i++){
            for(int j = i+1; j < nums.length; j++){
                if(nums[i] == nums[j]) count++;
            }
        }
      
        return count;
    }
}
```

---

# 8️⃣ How Many Numbers Are Smaller Than the Current Number — LC # 1365 Easy

```java
class Solution {
    public int[] smallerNumbersThanCurrent(int[] nums) {
        int[] res = new int[nums.length];
        for(int i = 0; i < nums.length; i++){
            int count = 0;
            for(int j=0; j<nums.length; j++){
                if(i!=j && nums[j] < nums[i]){
                    count++;
                }
            }
            res[i] = count;
        }
        return res;
    }
}
```

---

# 9️⃣ 

```java
class Solution {
    public int[] createTargetArray(int[] nums, int[] index) {
        ArrayList<Integer> list = new ArrayList<>();
        for(int i=0; i<nums.length; i++){
            list.add(index[i], nums[i]);
        }

        int[] target = new int[list.size()];
        for(int i=0; i<target.length; i++){
            target[i] = list.get(i);
        }
        return target;
    }
}
```

---

# 🔟 

```java
class Solution {
    public boolean checkIfPangram(String sentence) {
        boolean[] seen = new boolean[26];
        for(char c : sentence.toCharArray()){
            seen[c - 'a'] = true;
        }
        for(boolean s : seen){
            if(!s) return false;
        }
        return true;
    }
}
```