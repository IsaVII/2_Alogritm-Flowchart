![Lexicon Logo](https://lexicongruppen.se/media/wi5hphtd/lexicon-logo.svg)

# Workshop: Algorithm and Flowchart

For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### ✔ Pseudocode

```text
START
Sum = 0
FOR i = 1 TO 3 STEP +1
    INPUT Mark
    Sum = Sum + Mark
ENDFOR

Average = Sum / 3
PRINT Sum
PRINT Average

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[Sum = 0, i = 1]:::proc
    B --> C{i <= 3?}:::dec
    C --> |Yes| D[/INPUT Mark/]:::io
    D --> E[Sum += Mark, i++]:::proc
    E --> C
    
    C --> |No| F[Average=Sum/3]:::proc
    F --> G[/PRINT Sum, Average/]:::io
    G-->H([END]):::term
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode

```text
START
 
INPUT Number
FOR i = 1 TO 10 STEP +1
    Product = Number * i
    PRINT Product 
ENDFOR

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Number/]:::io
    B-->C[i = 1]:::proc
    C --> D{i <= 10?}:::dec

    D --> E[Product = Number*i, i++]:::proc
    E --> F[/PRINT Product/]
    F --> D
    D --> |No| G([END]):::term
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```
---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### ✔ Pseudocode

```text
START

INPUT Number
IF Number > 0
    PRINT Positive
ELSE IF Number < 0
    PRINT Negative
ELSE 
    PRINT Zero
ENDIF

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Number/]:::io
    B --> C{Number > 0?}:::dec
    C-->|Yes| D[/PRINT Positive/]:::io
    D --> E([END]):::term

    C-->|No| F{Number < 0}:::dec
    F-->|Yes| G[/PRINT Negative/]:::io
    G --> E

    F -->|No|H[/PRINT Zero/]:::io
    H-->E

 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode

```text
START
INPUT Money
INPUT Percentage
INPUT Years

Interest =  (Money * Percentage * Years) / 100
OUTPUT Interest
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Money/]:::io
    B --> C[/INPUT Percentage/]:::io
    C --> D[/INPUT Years/]:::io
    D --> E["Interest = (Money * Percentage * Years) / 100"]:::proc
    E --> F[/PRINT Interest/]:::io
    F --> G([END]):::term
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

### ✔ Pseudocode

```text
START
Sum = 0
FOR i = 1 TO 7  STEP +1
    INPUT Temperature
    Sum = Sum + Temperature
ENDFOR

Average = Sum / 7
PRINT Average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[Sum = 0, i = 1]:::proc
    B --> C{i <= 7?}:::dec
    C --> |Yes| D[/INPUT Temperature/]:::io
    D --> E[Sum += Temperature, i++]:::proc
    E --> C
    
    C --> |No| F[Average=Sum/7]:::proc
    F --> G[/PRINT Average/]:::io
    G-->H([END]):::term
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```
---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
START
INPUT Length
INPUT Width
Area = Length*Width
PRINT Area
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Length/]:::io
    B --> C[/INPUT Width/]:::io
    C --> D[Area = Length * Width]:::proc
    D --> E[/PRINT Area/]:::io
    E --> F([END]):::term
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```
---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode

```text
START
INPUT Average
IF Average >= 50
    PRINT Pass
ELSE
    PRINT FAIL
ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Average/]:::io
    B --> C{Average >= 50?}:::dec
    C -->|Yes| D[/PRINT "Pass"/]:::io
    D --> E([END]):::term

    C-->|No| F[/PRINT "Fail"/]:::io
    F --> E
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

```text
START
INPUT Number
Factorial = 1

FOR i = Number TO 1 STEP -1
    Factorial = FACTORIAL * i
ENDFOR

OUTPUT Factorial
END 
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Number/]:::io
    B --> C[Factorial = 1, i = Number]:::proc
    C --> D{i >= 1?}:::dec
    D -->|Yes| E[Factorial *= i, i--]:::proc
    E --> D

    D -->|No| F[/OUTPUT Factorial/]:::io
    F --> G([END]):::term
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### ✔ Pseudocode

```text
START
INPUT Amount
IF Amount > 1000
    Amount = Amount - Amount * 0.1
ENDIF

OUTPUT Amount
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Amount/]:::io
    B --> C{Amount > 1000}:::dec
    C -->|Yes| D["Apply Discount:
    Amount -= Amount * 0.1"]:::proc
    D --> E[/OUTPUT Amount/]:::io

    C -->|No| E
    E --> F([END]):::term
    
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## Optional Exercises (11–16)

## 11. Online Shopping Delivery Eligibility

Write the algorithm and draw the flowchart for a program that inputs a
customer's purchase amount and displays **"Free Delivery"** if the
amount is 500 SEK or more; otherwise display **"Delivery Charge
Applies"**.

### ✔ Pseudocode

```text
START
INPUT Amount
IF Amount >= 500
    PRINT Free Delivery
ELSE
    PRINT Delivery Charge Applies
ENDIF
 
END
 
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Amount/]:::io
    B --> C{Amount >= 500}:::dec
    C -->|Yes| D[/PRINT "Free Delivery"/]:::io
    D --> E([END]):::term

    C -->|No| F[/PRINT "Delivery Charge Applies"/]:::io
    F --> E
    
  
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 12. Employee Salary and Bonus Calculator

Write the algorithm and draw the flowchart for a program that inputs an
employee's monthly salary and years of service, calculates a bonus of
**10%** for employees with 5 or more years of service and **5%** for
others, then displays the bonus and total salary.

### ✔ Pseudocode

```text
START
INPUT Salary
INPUT ServiceYears
Rate = 0

IF ServiceYears >= 5
    Rate = 0.1
ELSE
    Rate = 0.05
ENDIF

Bonus = Rate * Salary
TotalSalary = Salary + Bonus
PRINT Bonus, TotalSalary
 
END
```

### ✔ Flowchart
```mermaid
flowchart TD
    A([START]):::term-->
    B[/INPUT Salary/]:::io
    B --> C[/INPUT ServiceYears/]:::io
    C --> D[Rate = 0]:::proc

    D --> E{ServiceYears >= 5}:::dec
    E -->|Yes| F[Rate = 0.1]:::proc
    E -->|No| K[Rate = 0.05]:::proc

    F --> G[Rate *= Salary]:::proc
    K --> G
    G --> H[TotalSalary = Salary + Bonus]:::proc
    H --> I[/PRINT Bonus, TotalSalary/]:::io
    I --> J([END]):::term
 
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
```

---

## 13. Mobile Data Usage Monitor

Write the algorithm and draw the flowchart for a program that inputs a
user's monthly data limit and data usage, then displays whether the user
has exceeded the limit or how much data remains.

### ✔ Pseudocode

```text
 
```

### ✔ Flowchart

---

## 14. Login System (Maximum 3 Attempts)

Create an algorithm and flowchart for a login system that allows a user
up to 3 attempts to enter the correct password. Display **"Access
Granted"** if the password is correct; otherwise display **"Account
Locked"** after 3 failed attempts.

### ✔ Pseudocode

```text
 
```

### ✔ Flowchart
---

## 15. Store Checkout with Multiple Items

Write the algorithm and draw the flowchart for a program that inputs the
number of items purchased, calculates the total purchase amount using a
loop, and applies a **15% discount** if the total exceeds 5000 SEK.

### ✔ Pseudocode

```text
 
```

### ✔ Flowchart

---

## 16. Electricity Bill Calculator

Write the algorithm and draw the flowchart for a program that inputs the
number of electricity units consumed and calculates the total bill using
the following rates: first 100 units at 1.5 SEK per unit, next 200
units at 2.0 SEK per unit, and all remaining units at 3.0 SEK per unit.

### ✔ Pseudocode

```text
 
```

### ✔ Flowchart

---
