# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Question

For

```math
A =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix},
```

compute:

```math
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
```

Explain the roles of the matrices I and 0, and describe the pattern you observe in successive powers of A.

## Solution

### 1. Identity and Zero Matrices

The appropriate matrices are:

```math
I =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix},
\qquad
0 =
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}.
```

Multiplying by I on either side leaves A unchanged:

```math
AI =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix},
```

```math
IA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}.
```

Adding the zero matrix also leaves A unchanged:

```math
A+0 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
+
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}.
```

Thus, I is the neutral element for matrix multiplication, and 0 is the neutral element for matrix addition.

### 2. Computing A² and A³

```math
A^2 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}.
```

```math
A^3 =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}.
```

### 3. Pattern in the Powers

The diagonal entries are powers of 2, the lower-left entry stays zero, and the upper-right entry follows n2ⁿ⁻¹:

```math
A^n =
\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n
\end{pmatrix},
\qquad n\geq1.
```

To explain the pattern, write:

```math
A=2I+N,
\qquad
N =
\begin{pmatrix}
0 & 1 \\
0 & 0
\end{pmatrix},
\qquad N^2=0.
```

Since I and N commute, the binomial expansion applies. All terms containing N² or higher powers vanish, giving:

```math
A^n=2^nI+n2^{n-1}N.
```
