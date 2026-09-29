
# Pseudocode-Flowchart Practice

## Pseudocode Practice
### Exercise 1: Find the Largest of Two Numbers (Decision)
Write the pseudocode for a program that:

Takes two numbers, A and B, as input.
Compares the two numbers.
Displays which number is larger.
If they are equal, display "Both numbers are equal."

```
Start 
Input A
Input B
If A > B  
    Display A
Else if A < B 
    Display B
Else 
    Display "Both numbers are equal" 
EndIf
End
```
---

### Exercise 2: Sum of 5 Numbers (Loop + Accumulation)
Write the pseudocode for a program that:

Reads 5 numbers one by one.
Calculates their total sum.
Displays the final result.

```
Start

Sum = 0
For 5 times
  Input Number 
  Sum += Number
End For

Display Sum
End
```
---
---
## Flowchart Practice

### Exercise 1: Voting Eligibility
Write a program that asks the user to enter their age.
- If the age is **18 or older**, display: "You are eligible to vote."
- If the age is **less than 18**, display: "You are not eligible to vote."
- End the program.

```mermaid
flowchart TD
    A([Start]):::term-->
    B[/Input Age/]:::io
    B --> C{Age >= 18?}:::proc
    C -- No --> D[/Output: "You are not eligible to vote."/]:::io
    C -- Yes --> E[/Output: "You are eligible to vote."/]:::io
    E --> F([End]):::term
    D--> F
  
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
  classDef pre fill:#ede7f6,stroke:#b39ddb,color:#333,stroke-width:1px;
  classDef conn fill:#f5f5f5,stroke:#bdbdbd,color:#333,stroke-width:1px;
  classDef hide fill:none,stroke:none,color:none;
  classDef label fill:none,stroke:none,color:#333,text-align:center;
```

---

### Exercise 2: Student Grade Calculator
Write a program that takes a student's marks (out of 100) as input and determines their grade:
- **90 or above:** "Grade A"
- **75 to 89:** "Grade B"
- **50 to 74:** "Grade C"
- **Below 50:** "Fail"
- End the program.

```mermaid
flowchart TD
    A([Start]):::term-->
    B[/Input Mark/]:::io

    B --> C{Mark >= 90?}:::dec
    C -- Yes --> D[/Output: "Grade A"/]:::io
    D-->End

    C -- No --> E{Mark >= 75}:::dec
    E -- Yes --> F[/Output: "Grade B"/]:::io
    F --> End

    E -- No --> G{Mark >= 50?}:::dec
    G -- Yes --> H[/Output: "Grade C"/]:::io
    H --> End
    G -- No --> I[/Output: "Fail"/]:::io
    I --> End

    End([End]):::term 
  
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
  classDef pre fill:#ede7f6,stroke:#b39ddb,color:#333,stroke-width:1px;
  classDef conn fill:#f5f5f5,stroke:#bdbdbd,color:#333,stroke-width:1px;
  classDef hide fill:none,stroke:none,color:none;
  classDef label fill:none,stroke:none,color:#333,text-align:center;
```
---

### Exercise 3: Simple Password Check
Write a program that:
1. Asks the user to enter a password.
2. Compares it with a stored password (e.g., "12345").
3. If they match, display: "Access Granted."
4. If they don't match, display: "Access Denied."
5. End the program.

```mermaid
flowchart TD
    A([Start]):::term-->
    B[/Input Password/]:::io

    B --> C{Match?}:::dec
    C -- Yes --> D[/Output: "Access Granted"/]:::io
    D-->End
    C -- No --> E[/Output: "Access Denied"/]:::io
    End([End]):::term 
  
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
  classDef pre fill:#ede7f6,stroke:#b39ddb,color:#333,stroke-width:1px;
  classDef conn fill:#f5f5f5,stroke:#bdbdbd,color:#333,stroke-width:1px;
  classDef hide fill:none,stroke:none,color:none;
  classDef label fill:none,stroke:none,color:#333,text-align:center;
```
---

### Exercise 4: Online Shopping Discount
Write a program that calculates the final price of an online order:
1. Input the **total purchase amount**.
2. If the amount is **5000 kr or more**, apply a **20% discount**.
3. If the amount is between **2000 kr and 4999 kr**, apply a **10% discount**.
4. If the amount is less than **2000 kr**, no discount is applied.
5. Calculate and display the **final price** after the discount.
6. End the program.


```mermaid
flowchart TD
    A([Start]):::term-->
    B[/Input Total/]:::io

    B --> C{Total >= 5000?}:::dec
    C -- Yes --> D[Discount 20%]:::proc
    D-->F[/Output: Final Price/]:::io
    F-->End

    C -- No --> G{Total >= 2000?}:::dec
    G -- Yes --> H[Discount 10%]:::proc
    H-->F

    G -- No --> F


    End([End]):::term 
  
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
  classDef pre fill:#ede7f6,stroke:#b39ddb,color:#333,stroke-width:1px;
  classDef conn fill:#f5f5f5,stroke:#bdbdbd,color:#333,stroke-width:1px;
  classDef hide fill:none,stroke:none,color:none;
  classDef label fill:none,stroke:none,color:#333,text-align:center;
```
---

#### Exercise 5: Smart Parking Fee Calculator
Write a program that calculates the parking fee for a city garage:
1.  Ask the user for the **number of hours** parked (e.g., 4).
2.  If the time is **1 hour or less**, the fee is **0 kr** (Free).
3.  If the time is **between 1 and 3 hours**, the fee is a flat **50 kr**.
4.  If the time is **more than 3 hours**, calculate the fee as: **50 kr + (40 kr for every hour beyond the 3rd hour)**.
5.  If the calculated fee is **greater than 250 kr**, set the fee to **250 kr** (Maximum Daily Rate).
6.  Ask if the user has a **"Loyalty Card"**. If **Yes**, subtract **20%** from the fee.
7.  Display the **Final Fee** and end the program.

```mermaid
flowchart TD
    A([Start]):::term-->
    B[/Input Park-Hours/]:::io

    B --> C{Park-Hours <= 1?}:::dec
    C -- Yes --> D[Final Fee=0 kr]:::proc
    D-->Out
   

    C -- No --> G{Park-Hours <= 3?}:::dec
    G -- Yes --> H[Final Fee=50 kr]:::proc
    H-->LC

    G -- No --> J[Final Fee=
    50 kr + /Hours-3/ * 40 kr]:::proc
    J--> K{Final Fee > Daily Rate /250/}:::dec
    K -- No --> LC
    
    K -- Yes --> L[Final Fee = Daily Rate]:::proc  
    L --> LC[/Input Loyalty/]:::io
    LC --> M{Loyalty?}:::dec
    M-- Yes --> N[20% Discount]:::proc  

     N --> Out[/Output Final Fee/]:::io
     M -- No --> Out
     Out --> End

 
    End([End]):::term 
  
  classDef term fill:#e3f2fd,stroke:#90caf9,color:#333,stroke-width:1px;
  classDef io fill:#fff3e0,stroke:#ffcc80,color:#333,stroke-width:1px;
  classDef proc fill:#e8f5e9,stroke:#a5d6a7,color:#333,stroke-width:1px;
  classDef dec fill:#fde0dc,stroke:#f8bbd0,color:#333,stroke-width:1px;
  classDef pre fill:#ede7f6,stroke:#b39ddb,color:#333,stroke-width:1px;
  classDef conn fill:#f5f5f5,stroke:#bdbdbd,color:#333,stroke-width:1px;
  classDef hide fill:none,stroke:none,color:none;
  classDef label fill:none,stroke:none,color:#333,text-align:center;
```