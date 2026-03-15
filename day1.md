# Basic Programming Problems – Flowchart and Pseudocode

This document contains **Flowcharts and Pseudocode** for beginner programming problems.

---

# 1️⃣ Leap Year Check

## Flowchart

```mermaid
flowchart TD
A[Start] --> B[Input Year]
B --> C{Year % 4 == 0?}
C -- No --> D[Not Leap Year]
C -- Yes --> E{Year % 100 != 0 OR Year % 400 == 0?}
E -- Yes --> F[Leap Year]
E -- No --> D
F --> G[End]
D --> G
```

## Pseudocode

```
START
INPUT year

IF year % 4 == 0 THEN
    IF year % 100 != 0 OR year % 400 == 0 THEN
        PRINT "Leap Year"
    ELSE
        PRINT "Not Leap Year"
    ENDIF
ELSE
    PRINT "Not Leap Year"
ENDIF

END
```

---

# 2️⃣ Sum of Two Numbers

## Flowchart

```mermaid
flowchart TD
A[Start] --> B[Input Number1]
B --> C[Input Number2]
C --> D[Sum = Number1 + Number2]
D --> E[Print Sum]
E --> F[End]
```

## Pseudocode

```
START

INPUT number1
INPUT number2

sum = number1 + number2

PRINT sum

END
```

---

# 3️⃣ Multiplication Table

## Flowchart

```mermaid
flowchart TD
A[Start] --> B[Input Number]
B --> C[Set i = 1]
C --> D{i ≤ 10 ?}
D -- No --> H[End]
D -- Yes --> E[Print number × i]
E --> F[i = i + 1]
F --> D
```

## Pseudocode

```
START

INPUT number
SET i = 1

WHILE i <= 10
    PRINT number × i
    i = i + 1
END WHILE

END
```

---

# 4️⃣ HCF and LCM

## Flowchart

```mermaid
flowchart TD
A[Start] --> B[Input a, b]
B --> C[x = a, y = b]
C --> D{y ≠ 0 ?}
D -- No --> E[HCF = x]
D -- Yes --> F[temp = y]
F --> G[y = x % y]
G --> H[x = temp]
H --> D
E --> I[LCM = (a × b) / HCF]
I --> J[Print HCF and LCM]
J --> K[End]
```

## Pseudocode

```
START

INPUT a
INPUT b

x = a
y = b

WHILE y ≠ 0
    temp = y
    y = x % y
    x = temp
END WHILE

HCF = x
LCM = (a * b) / HCF

PRINT HCF
PRINT LCM

END
```

---

# 5️⃣ Sum Until 'x'

## Flowchart

```mermaid
flowchart TD
A[Start] --> B[sum = 0]
B --> C[Input value]
C --> D{value == x ?}
D -- Yes --> F[Print sum]
F --> G[End]
D -- No --> E[sum = sum + value]
E --> C
```

## Pseudocode

```
START

sum = 0

REPEAT
    INPUT value

    IF value == 'x'
        BREAK
    ENDIF

    sum = sum + value

UNTIL value == 'x'

PRINT sum

END
```
