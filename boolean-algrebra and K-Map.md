### What is Boolean Algebra?

Boolean algebra is also known as binary algebra or logical algebra. Venn diagrams can be used
to get a visual representation of any Boolean algebra operation. The variables used in Boolean
Algebra only have one of two possible values, a logic “0” and a logic “1” but an expression can
have an infinite number of variables.

- `0` represents `false`, (or `off` is represented by `0`)
- `1` represents `true`, (or `on` is represented by `1`)

### Boolean Function?
A function that contains **boolean variables** (𝐴, 𝐵, 𝐶, etc.) and their **compliments** (𝐴', 𝐵', 𝐶', etc.) with **boolean operations** (`+`, `.`) is called boolean function.
e.g.,   f(A,B,C) = AB' + B'C + CA  
<br>
**!Important Note:** Number of maximum boolean functions can be formed using `n` boolean variables = **2<sup>2<sup>n</sup></sup>**

**Ques. How many boolean functions can be formed using one boolean variable?**  
Number of boolean function can be formed using n boolean variable is = 2<sup>2<sup>n</sup></sup>  
then, 
number of boolean function can be formed using 1 boolean variable = 2<sup>2<sup>1</sup></sup> = 2<sup>2</sup> = 4.  
for example: let suppose `X` is boolean variable then possible boolean functions is  
- f(X) = X
- f(X) = X'
- f(X) = X + X'
- f(X) = X . X'

**Ques. How many maximum boolean functions can be formed using 3 boolean variables X, Y, Z ?**  
**Ans.** 2<sup>2<sup>3</sup></sup> = 2<sup>8</sup> = 256.

**Ques. There are maximum 2048 boolean functions, How many different variables are used ?**  
&emsp; a) 12  
&emsp; b) 6   
&emsp; c) 11  
&emsp; d) None  <br>
**Ans.** 2<sup>2<sup>n</sup></sup> = 2048      
2<sup>2<sup>n</sup></sup> = 2<sup>11</sup>  
2<sup>n</sup> = 11  (n ∈ N)  
_correct option (d) none_

### Representation of Boolean Functions? 
There are two standard ways to represent boolean functions --   
1. **Sum of Products (SOP):**
   - A = 0 is represented as A' and A = 1 will be represented as A
   - It is also called **Disjunctive Normal Form (DNF)**.
   - Each term in SOP is called a **minterm**.
   - **e.g.,** F = (A ⋅ B) + (B ⋅ C) + (A ⋅ C) <br> 𝐹 = 𝐴𝐵'𝐶 + 𝐴𝐵𝐶' + 𝐴𝐵𝐶
   - The **Σ (Sigma)** symbol is used to denote the sum of minterms. <br> **Representation** F(A, B, C) = Σm(0, 1, 3, 7)
3. **Product of Sums (POS):**
   - A = 0 is represented as A and A = 1 will be represented as A'.
   - It is also called **Conjunctive Normal Form (CNF)**.
   - Each term in POS is called a **maxterm**.
   - **e.g.,** F = (A + B) . (B + C) . (A + C) <br> F = (A' + B + C) . (A + B' + C').
   - The **&pi; (Pi) symbol** is used to denote the product of maxterms. <br> **Representation** F(A, B, C) = &pi;M(2, 4, 5, 6)

### Minimization of Boolean Functions?   
Minimization is the process of reducing a Boolean function to its simplest (smallest) form, which helps in designing optimized logic circuits. The main methods used for Boolean function minimization are:
1. **Using Boolean Algebra:** This method uses Boolean laws and theorems to simplify expressions manually.
2. **Using Karnaugh Map (K-map) Method:** A K-map is a graphical way to minimize Boolean expressions for up to 4 or 5 variables.

**Important Results:**
- Complete SOP boolean function Always gives result `1`.   
  e.g., For two variables complete SOP: &nbsp;  F(A, B) = AB + A'B + AB' + A'B' <br>
  **Minimize** <br> = AB + A'B + AB' + A'B' <br> = B(A + A') + B'(A + A') <br> = B.1 + B'.1 <br> = B + B' <br> = 1
- Complete POS boolean function Always gives result `0`.   
  e.g., For two variables complete POS: &nbsp; F(A, B) = (A + B)(A + B')(A' + B)(A' + B') <br>

### Boolean Algebra Operators?
Boolean Algebra consists of fundamental operators used in logic circuits, programming, and mathematical expressions.

| **Operator** | **Symbol** | **Procedure Name** | **Name**        | **Truth Table Example**     |
|--------------|-----------|---------------------|-----------------|-----------------------------|
| AND        | `.` (or `∧`) | Intersection or <br>Multiplication  | Conjunction     |  `A . B = Y` <br> `0 . 0 = 0` <br> `0 . 1 = 0` <br> `1 . 0 = 0` <br> `1 . 1 = 1` |
| OR         | `+` (or `∨`) | Union or <br>Addition  | Disjunction        |  `A + B = Y` <br> `0 + 0 = 0` <br> `0 + 1 = 1` <br> `1 + 0 = 1` <br> `1 + 1 = 1` |
| NOT        | `'` or `¯` (or `¬`) | Complement or <br> Inversion | Negation           | `A' = Y` <br> `0' = 1` <br> `1' = 0` |
| NAND       | ↑            |         | NOT AND            |  `A ↑ B = Y` <br> `0 ↑ 0 = 1` <br> `0 ↑ 1 = 1` <br> `1 ↑ 0 = 1` <br> `1 ↑ 1 = 0` |
| XOR        | ⊕           |         | Exclusive OR      |  `A ⊕ B = Y` <br> `0 ⊕ 0 = 0` <br> `0 ⊕ 1 = 1` <br> `1 ⊕ 0 = 1` <br> `1 ⊕ 1 = 0` |
| NOR        | ↓            |         | NOT OR             |  `A ↓ B = Y` <br> `0 ↓ 0 = 1` <br> `0 ↓ 1 = 0` <br> `1 ↓ 0 = 0` <br> `1 ↓ 1 = 0` |
| XNOR       | ⊙           |         | Exclusive NOR     |  `A ⊙ B = Y` <br> `0 ⊙ 0 = 1` <br> `0 ⊙ 1 = 0` <br> `1 ⊙ 0 = 0` <br> `1 ⊙ 1 = 1` |

📝 **Important Note:**

- **AND (.)**: True when both inputs are **true**.
- **OR (+)**: True when at least **one** input is **true**.
- **NOT (¯ or ')**: Inverts the input.
- **XOR (⊕)**: True when inputs are **different**.
- **NAND (↑)**: True unless both inputs are **true**.
- **NOR (↓)**: True when both inputs are **false**.
- **XNOR (⊙)**: True when inputs are **the same**.

📝 **Important Equatios:**

| **Operator** | **Equation** | 
|--------------|-------------|
| AND | A . B |
| OR  | A + B |
| NOT | A' |
| NAND | (A . B)' |
| NOR | (A + B)' |
| XOR | A ⊕ B = A'B + B'A <br> A ⊕ A = 0 <br> 0 ⊕ A = A |
| XNOR | A ⊙ B = (A ⊕ B)' <br> (A ⊕ B)' = (A'B + B'A)' <br> A ⊙ B = (A + B') . (B + A') |
| SOP | SOP = (POS)' |
| POS | POS = (SOP)' |
| TRUE (Tautology) | 1 |
| FALSE (Contradiction or falsy) | 0 |

📝 **Set Representation in Boolean Equation:**

| **Set** | **Boolean Equation** | 
|--------------|-------------|
| A - B | AB' |
| B - A  | BA' |
| A 🔺 B | A ⊕ B or AB' + BA' |
| A ∪ B | A + B |
| A ∩ B | A . B |

### Basic logic gates

<img src="./assets/images/basic-gates.png" width="600px"/>

### Laws of Boolean Algebra

| **Name of Law**  | **AND Form** | **OR Form** | 
|------------------|--------------|-------------|
| Identity law     | 𝐴 . 1 = 𝐴     | 𝐴 + 0 = 𝐴   |
| Null law         | 𝐴 . 0 = 0     | 𝐴 + 1 = 1   |
| Idempotent law   | 𝐴 . 𝐴 = 𝐴     | 𝐴 + 𝐴 = 𝐴  |  
| Inverse law      | 𝐴 . 𝐴' = 0     | 𝐴 + 𝐴'= 1    | 
| Commutative law  | 𝐴 . 𝐵 = 𝐵 . 𝐴   | 𝐴 + 𝐵 = 𝐵 + 𝐴 | 
| Associative law  | 𝐴 . (𝐵 . 𝐶) = (𝐴 . 𝐵) . 𝐶    |    𝐴 + (𝐵 + 𝐶) = (𝐴 + 𝐵) + 𝐶 |  
| Distributive law | 𝐴 . (𝐵 + 𝐶) = 𝐴 . 𝐵 + 𝐴 . 𝐶   | 𝐴 + (𝐵𝐶) = (𝐴 + 𝐵)(𝐴 + 𝐶)    | 
| Absorption law   | 𝐴(𝐴 + 𝐵) = 𝐴  <br> 𝐴 . (𝐴' + 𝐵) = 𝐴 . 𝐵   |  𝐴 + 𝐴𝐵 = 𝐴  <br> 𝐴 + (𝐴' . 𝐵) = 𝐴 + 𝐵     | 
| Other            | (𝐴')' = 𝐴 <br> .' = + | <br>  +' = `.`     |
| De Morgan's law  | (AB)' = A' + B' <br> (ABC...)' = A' + B' + C' + ...  |  (A + B)' = A' . B' <br> (A + B + C + ...)' = A' . B' . C' . ... | 


### Questions and Solutions.

<img src="./assets/images/Boolean_algebra_ques_1.png" />
<img src="./assets/images/Boolean_algebra_ques_2.png" />
<img src="./assets/images/Boolean_algebra_ques_3.png" />


## K-Map (Karnaugh Map) Method: 
In many digital circuits and practical problems, we need to find expressions with minimum variables. We can minimize Boolean expressions of 3, 4 variables very easily using K-map without using any Boolean algebra theorems.   
Number of cells in K-map = number of possible cases   
No. of possible cases = 2<sup>n</sup>   
n -> is the number of input variables.   
K-map can take two forms:
1. Sum of product (SOP)
2. Product of Sum (POS)

### How to create K-Map for Sum of product (SOP) and Product of Sum (POS)

**A) K-Map for two variables:** In the 2 variable k-map, 4 (2<sup>2</sup>) squares are required. Each square contains one term of expression with two variables.    
<img src="./assets/images/2-variables-k-map.png" width="400px"/>

**B) K-Map for three variables:** In the three variable k-map, 8 (2<sup>3</sup>) square is required. The 3-variables k-map can content either horizontally or vertically.    
<img src="./assets/images/3-variables-k-map.png" width="400px"/>

**C) K-Map for four variables:** In the 4 variable k-map, 16 (2<sup>4</sup>) square are required.    
<img src="./assets/images/4-variables-k-map.png" width="600px"/>


### How to insert SOP representation of Boolean Function into k-map?












