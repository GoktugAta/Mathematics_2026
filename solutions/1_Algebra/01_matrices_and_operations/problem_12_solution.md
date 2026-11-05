# Exercise 12. Formula for a Matrix Power

## Question

Let

```math
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}.
```

Compute A², A³, and A⁴, and use them to formulate a conjecture for Aⁿ. Then do not stop after checking one more case: assume the formula is true for n, multiply by A, and explain why you obtain exactly the formula for n + 1.

## Solution

### 1. Computing the First Powers

```math
A^2 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}.
```

```math
A^3 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}.
```

```math
A^4 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}.
```

### 2. Conjecture

The diagonal entries remain 1, the lower-left entry remains 0, and the upper-right entry increases by 1 at each step. We conjecture:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix},
\qquad n\geq1.
```

### 3. Proof by Induction

For n = 1, the formula gives A itself, so the base case holds.

Assume the formula is true for some integer n ≥ 1. Multiplying by A gives:

```math
A^{n+1}=A^nA
=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 1+n \\
0 & 1
\end{pmatrix}.
```

This is exactly the same formula with n replaced by n + 1. Therefore, mathematical induction proves the formula for every integer n ≥ 1.
