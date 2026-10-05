# Workshop: Algorithm and Flowchart — Solutions

## 1. Check Even or Odd Number
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
### ✔ Pseudocode
```text
START
    INPUT Mark1, Mark2, Mark3
    Total = Mark1 + Mark2 + Mark3
    Average = Total / 3
    PRINT Total
    PRINT Average
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input 3 Marks/]
    B --> C[Calculate Total]
    C --> D[Calculate Average]
    D --> E[/Display Total and Average/]
    E --> F([End])
```
---

## 3. Display Multiplication Table
### ✔ Pseudocode
```text
START
    INPUT Number
    FOR I = 1 TO 10
        PRINT Number * I
    NEXT I
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input Number/]
    B --> C[I = 1]
    C --> D{I <= 10?}
    D -->|Yes| E[/Display Number × I/]
    E --> F[I = I + 1]
    F --> D
    D -->|No| G([End])
```
---

## 4. Positive, Negative, or Zero Check
### ✔ Pseudocode
```text
START
    INPUT Number
    IF Number > 0 THEN
        PRINT "Positive"
    ELSE IF Number < 0 THEN
        PRINT "Negative"
    ELSE
        PRINT "Zero"
    ENDIF
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input Number/]
    B --> C{Number > 0?}
    C -->|Yes| D[/Positive/]
    C -->|No| E{Number < 0?}
    E -->|Yes| F[/Negative/]
    E -->|No| G[/Zero/]
    D --> H([End])
    F --> H
    G --> H
```
---

## 5. Simple Interest Calculator
### ✔ Pseudocode
```text
START
    INPUT P, R, T
    SI = (P * R * T) / 100
    PRINT SI
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input P, R, T/]
    B --> C[Calculate SI]
    C --> D[/Display SI/]
    D --> E([End])
```
---

## 6. Average Temperature Calculation
### ✔ Pseudocode
```text
START
    Total = 0
    FOR Day = 1 TO 7
        INPUT Temp
        Total = Total + Temp
    NEXT Day
    Average = Total / 7
    PRINT Average
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[Total = 0, Day = 1]
    B --> C{Day <= 7?}
    C -->|Yes| D[/Input Temperature/]
    D --> E[Add to Total]
    E --> F[Day = Day + 1]
    F --> C
    C -->|No| G[Average = Total / 7]
    G --> H[/Display Average/]
    H --> I([End])
```
---

## 7. Calculate Area of a Rectangle
### ✔ Pseudocode
```text
START
    INPUT Length, Width
    Area = Length * Width
    PRINT Area
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input Length and Width/]
    B --> C[Area = Length * Width]
    C --> D[/Display Area/]
    D --> E([End])
```
---

## 8. Determine Pass or Fail
### ✔ Pseudocode
```text
START
    INPUT Average
    IF Average >= 50 THEN
        PRINT "Pass"
    ELSE
        PRINT "Fail"
    ENDIF
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input Average/]
    B --> C{Average >= 50?}
    C -->|Yes| D[/Pass/]
    C -->|No| E[/Fail/]
    D --> F([End])
    E --> F
```
---

## 9. Calculate Factorial of a Number
### ✔ Pseudocode
```text
START
    INPUT N
    Factorial = 1
    FOR I = 1 TO N
        Factorial = Factorial * I
    NEXT I
    PRINT Factorial
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input N/]
    B --> C[Factorial = 1, I = 1]
    C --> D{I <= N?}
    D -->|Yes| E[Factorial = Factorial * I]
    E --> F[I = I + 1]
    F --> D
    D -->|No| G[/Display Factorial/]
    G --> H([End])
```
---

## 10. Calculate Discount on Purchase
### ✔ Pseudocode
```text
START
    INPUT Amount
    IF Amount > 1000 THEN
        Discount = Amount * 0.10
    ELSE
        Discount = 0
    ENDIF
    Final = Amount - Discount
    PRINT Final
END
```
### ✔ Flowchart
```mermaid
flowchart TD
    A([Start]) --> B[/Input Amount/]
    B --> C{Amount > 1000?}
    C -->|Yes| D[Calculate 10% Discount]
    C -->|No| E[Discount = 0]
    D --> F[Calculate Final Amount]
    E --> F
    F --> G[/Display Final Amount/]
    G --> H([End])
```
---

## 11. Online Shopping Delivery Eligibility

### ✔ Pseudocode

```text
START

    INPUT PurchaseAmount

    IF PurchaseAmount >= 500 THEN
        PRINT "Free Delivery"
    ELSE
        PRINT "Delivery Charge Applies"
    ENDIF

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Purchase Amount/]
    B --> C{Amount >= 500?}
    C -->|Yes| D[/Display Free Delivery/]
    C -->|No| E[/Display Delivery Charge Applies/]
    D --> F([End])
    E --> F
```

---

## 12. Employee Salary and Bonus Calculator

### ✔ Pseudocode

```text
START

    INPUT Salary
    INPUT YearsOfService

    IF YearsOfService >= 5 THEN
        Bonus = Salary * 0.10
    ELSE
        Bonus = Salary * 0.05
    ENDIF

    TotalSalary = Salary + Bonus

    PRINT Bonus
    PRINT TotalSalary

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Salary and Years of Service/]
    B --> C{Years >= 5?}
    C -->|Yes| D[Bonus = Salary × 10%]
    C -->|No| E[Bonus = Salary × 5%]
    D --> F[Total Salary = Salary + Bonus]
    E --> F
    F --> G[/Display Bonus and Total Salary/]
    G --> H([End])
```

---

## 13. Mobile Data Usage Monitor

### ✔ Pseudocode

```text
START

    INPUT DataLimit
    INPUT DataUsed

    IF DataUsed > DataLimit THEN
        Extra = DataUsed - DataLimit
        PRINT "Data Limit Exceeded"
        PRINT Extra
    ELSE
        Remaining = DataLimit - DataUsed
        PRINT "Data Remaining"
        PRINT Remaining
    ENDIF

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Data Limit and Data Used/]
    B --> C{Data Used > Data Limit?}

    C -->|Yes| D[Extra = Used - Limit]
    D --> E[/Display Data Limit Exceeded and Extra Usage/]

    C -->|No| F[Remaining = Limit - Used]
    F --> G[/Display Data Remaining/]

    E --> H([End])
    G --> H
```

---

## 14. Login System (Maximum 3 Attempts)

### ✔ Pseudocode

```text
START

    Password = "admin123"
    Attempts = 0

    WHILE Attempts < 3

        INPUT UserPassword

        IF UserPassword = Password THEN
            PRINT "Access Granted"
            STOP
        ENDIF

        Attempts = Attempts + 1

    ENDWHILE

    PRINT "Account Locked"

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Set Password and Attempts = 0]
    B --> C{Attempts < 3?}

    C -->|Yes| D[/Input Password/]
    D --> E{Password Correct?}

    E -->|Yes| F[/Display Access Granted/]
    F --> G([End])

    E -->|No| H[Attempts = Attempts + 1]
    H --> C

    C -->|No| I[/Display Account Locked/]
    I --> G
```

---

## 15. Store Checkout with Multiple Items

### ✔ Pseudocode

```text
START

    INPUT NumberOfItems

    Total = 0
    Counter = 1

    WHILE Counter <= NumberOfItems

        INPUT Price
        Total = Total + Price

        Counter = Counter + 1

    ENDWHILE

    IF Total > 5000 THEN
        Discount = Total * 0.15
    ELSE
        Discount = 0
    ENDIF

    FinalAmount = Total - Discount

    PRINT Total
    PRINT Discount
    PRINT FinalAmount

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Number of Items/]
    B --> C[Total = 0, Counter = 1]

    C --> D{Counter <= NumberOfItems?}

    D -->|Yes| E[/Input Item Price/]
    E --> F[Total = Total + Price]
    F --> G[Counter = Counter + 1]
    G --> D

    D -->|No| H{Total > 5000?}

    H -->|Yes| I[Discount = 15% of Total]
    H -->|No| J[Discount = 0]

    I --> K[Final Amount = Total - Discount]
    J --> K

    K --> L[/Display Total, Discount and Final Amount/]
    L --> M([End])
```

---

## 16. Electricity Bill Calculator

### ✔ Pseudocode

```text
START

    INPUT Units

    IF Units <= 100 THEN
        Bill = Units * 1.5

    ELSE IF Units <= 300 THEN
        Bill = (100 * 1.5) +
               ((Units - 100) * 2.0)

    ELSE
        Bill = (100 * 1.5) +
               (200 * 2.0) +
               ((Units - 300) * 3.0)
    ENDIF

    PRINT Bill

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Units Consumed/]

    B --> C{Units <= 100?}

    C -->|Yes| D["Bill = Units * 1.5"]

    C -->|No| E{Units <= 300?}

    E -->|Yes| F["Bill = (100 * 1.5) + ((Units - 100) * 2.0)"]

    E -->|No| G["Bill = (100 * 1.5) + (200 * 2.0) + ((Units - 300) * 3.0)"]

    D --> H[/Display Bill/]
    F --> H
    G --> H

    H --> I([End])
```
