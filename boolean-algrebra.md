### What is Boolean Algebra?

Boolean algebra is also known as binary algebra or logical algebra. Venn diagrams can be used
to get a visual representation of any Boolean algebra operation. The variables used in Boolean
Algebra only have one of two possible values, a logic “0” and a logic “1” but an expression can
have an infinite number of variables.

- `0` represents `false`, (or `off` is represented by `0`)
- `1` represents `true`, (or `on` is represented by `1`)

### Boolean Algebra Operators?

Boolean Algebra consists of fundamental operators used in logic circuits, programming, and mathematical expressions.

| **Operator** | **Symbol** | **Procedure Name** | **Name**        | **Truth Table Example**     |
|-------------|-----------|---------------------|-------------------|-----------------------------|
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

### Basic logic gates

![Basic Gates](./assets/images/basic-gates.png)

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





