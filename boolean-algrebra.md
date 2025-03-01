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
| AND        | `.` (or `∧`) | Intersection or <br>Multiplication  | Conjunction        |  `A . B` <br> `0 . 0 = 0` <br> `0 . 1 = 0` <br> `1 . 0 = 0` <br> `1 . 1 = 1` |
| OR         | `+` (or `∨`) | Union or <br>Addition  | Disjunction        |  `A + B` <br> `0 + 0 = 0` <br> `0 + 1 = 1` <br> `1 + 0 = 1` <br> `1 + 1 = 1` |
| NOT        | `'` or `¯` (or `¬`) | Complement or <br> Inversion | Negation           | `A'` <br> `0' = 1` <br> `1' = 0` |
| NAND       | ↑            |         | NOT AND            |  `A ↑ B` <br> `0 ↑ 0 = 1` <br> `0 ↑ 1 = 1` <br> `1 ↑ 0 = 1` <br> `1 ↑ 1 = 0` |
| XOR        | ⊕           |         | Exclusive OR      |  `A ⊕ B` <br> `0 ⊕ 0 = 0` <br> `0 ⊕ 1 = 1` <br> `1 ⊕ 0 = 1` <br> `1 ⊕ 1 = 0` |
| NOR        | ↓            |         | NOT OR             |  `A ↓ B` <br> `0 ↓ 0 = 1` <br> `0 ↓ 1 = 0` <br> `1 ↓ 0 = 0` <br> `1 ↓ 1 = 0` |
| XNOR       | ⊙           |         | Exclusive NOR     |  `A ⊙ B` <br> `0 ⊙ 0 = 1` <br> `0 ⊙ 1 = 0` <br> `1 ⊙ 0 = 0` <br> `1 ⊙ 1 = 1` |

> [!IMPORTANT]

- **AND (.)**: True when both inputs are **true**.
- **OR (+)**: True when at least **one** input is **true**.
- **NOT (¯ or ')**: Inverts the input.
- **XOR (⊕)**: True when inputs are **different**.
- **NAND (↑)**: True unless both inputs are **true**.
- **NOR (↓)**: True when both inputs are **false**.
- **XNOR (⊙)**: True when inputs are **the same**.




### Basic logic gates

![Basic Gates](./assets/images/basic-gates.png)

## Notation and definitions

- *Complement*: opposite of a variable value
- *Multiplication*: represent bit-wise AND
- *Addition*: represent bit-wise OR
- *Operator precedence*: `NOT > AND > OR`
- *Input variables*: represent a binary input value
- *Output variables*: evaluation of a boolean expression represents a binary output value
- *Literal*: each occurance of a variable in the expression
- *Term*: minimum unit of the expression. The form determines the first-level gate unit

## Boolean identities

> The key to simplifying Boolean expressions is to learn the Identities

### Basic identities

- Double complement: $(A')' = A$
- Idempotence: $A \cdot A = A$ or $A + A = A$
- Inverse: $A \cdot A' = 0$ or $A + A' = 1$
- Null (or dominance): $A \cdot 0 = 0$ or $A + 1 = A$
- Identity: $A \cdot 1 = A$ or $A + 0 = A$
- Distributive: $A \cdot (B + C) = A \cdot B + A \cdot C$ or $A + (B \cdot C) = (A + B) \cdot (A + C)$
- Commutative: $A \cdot B = B \cdot A$ or $A + B = B + A$
- Assosiative: $(A \cdot B) \cdot C = A \cdot (B \cdot C)$ or $(A + B) + C = A + (B + C)$

**Note:** .' = + and +' = .

### Advanced identities

- Note that $A$ and $B$ could refer to any complex Boolean expression

#### Absorption law

- $A + (A \cdot B) = A$
- $(A) \cdot (A + B) = A$

#### No-name

- $A + A' \cdot B = A + B$
- $A(A' + B) = A \cdot B$

#### Consensus

- $AB + BC + A'C = AB + A'C$
- $(A + B)(B + C)(A' + C) = (A + B)(A' + C)$

#### De Morgan's law

- $(A + B)' = A' \cdot B'$
- $(A \cdot B)' = A' + B'$
- This holds for any number of terms

## Equivalent representations

- Boolean functions and expressions can be *expressed* in different ways
- *Boolean expression*: the logical expression
- *Gate diagrams*: expressed as a term of logical operations and wires
- *Truth tables*: express output in terms of all possible combination of its input
