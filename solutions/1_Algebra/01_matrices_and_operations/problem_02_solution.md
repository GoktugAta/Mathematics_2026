# Exercise 2. Addition and Scalar Multiplication

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix},
```

compute:

```math
A+B,\qquad A-B,\qquad 3A-2B.
```

Explain why matrix addition is possible only for matrices of the same size.

## Solution

### 1. Computing A + B

Matrix addition is performed entry by entry:

```math
A+B =
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}.
```

### 2. Computing A − B

Subtract corresponding entries:

```math
A-B =
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}.
```

### 3. Computing 3A − 2B

First multiply every entry by the corresponding scalar:

```math
3A =
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix},
\qquad
2B =
\begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}.
```

Then subtract:

```math
3A-2B =
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}.
```

### 4. Why Equal Sizes Are Required

Matrix addition pairs each entry of one matrix with the entry in the same row and column of the other matrix. Therefore, both matrices must have the same number of rows and columns so that every entry has a corresponding partner.
