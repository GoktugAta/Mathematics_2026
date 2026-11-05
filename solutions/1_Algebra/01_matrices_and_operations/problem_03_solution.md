# Exercise 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are:

```math
A_{2\times3},
\qquad
B_{3\times4},
\qquad
C_{4\times2},
\qquad
D_{2\times2}.
```

For the products

```math
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA,
```

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

### Dimension Compatibility Rule

A product MN is defined when the number of columns of M equals the number of rows of N.

If M has size m × n and N has size n × p, then MN has size m × p.

### Checking Each Product

| Product | Factor sizes | Compatibility check | Result |
|---|---|---|---|
| AB | (2 × 3)(3 × 4) | 3 = 3 | Defined; 2 × 4 |
| BA | (3 × 4)(2 × 3) | 4 ≠ 2 | Not defined |
| BC | (3 × 4)(4 × 2) | 4 = 4 | Defined; 3 × 2 |
| CB | (4 × 2)(3 × 4) | 2 ≠ 3 | Not defined |
| AC | (2 × 3)(4 × 2) | 3 ≠ 4 | Not defined |
| CA | (4 × 2)(2 × 3) | 2 = 2 | Defined; 4 × 3 |
| AD | (2 × 3)(2 × 2) | 3 ≠ 2 | Not defined |
| DA | (2 × 2)(2 × 3) | 2 = 2 | Defined; 2 × 3 |

Thus, the defined products are AB, BC, CA, and DA. Their sizes come from the outer dimensions of the two factors.
