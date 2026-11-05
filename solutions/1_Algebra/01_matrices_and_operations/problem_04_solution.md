# Exercise 4. Matrix Multiplication and Noncommutativity

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix},
```

compute AB and BA. Is AB = BA? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

### 1. Computing AB

Each entry is the dot product of a row of A and a column of B:

```math
AB =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1
\end{pmatrix}
=
\begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}.
```

### 2. Computing BA

```math
BA =
\begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1
\end{pmatrix}
=
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}.
```

### 3. Comparison

```math
\begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}.
```

Therefore, AB ≠ BA.

### 4. Meaning of Noncommutativity

Matrix multiplication is generally noncommutative: changing the order of the factors can change the result. In this example, both products are defined, but AB and BA are different matrices.
