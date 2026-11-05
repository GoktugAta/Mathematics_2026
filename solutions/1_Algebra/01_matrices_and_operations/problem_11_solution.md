# Exercise 11. When Do Matrices Commute?

## Question

Given

```math
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
```

find the conditions on a, b, c, d under which AB = BA. Describe the general form of all such matrices B.

## Solution

### 1. Computing Both Products

```math
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}.
```

```math
BA =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}.
```

### 2. Equating Corresponding Entries

For AB = BA, corresponding entries must be equal:

```math
\begin{cases}
a+c=a, \\
b+d=a+b, \\
c=c, \\
d=c+d.
\end{cases}
```

The first and fourth equations require c = 0. The second requires d = a. The third gives no additional restriction.

Thus, the necessary conditions are:

```math
c=0,\qquad d=a.
```

### 3. General Form and Verification

The general form is:

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix},
\qquad a,b\in\mathbb{R}.
```

Substituting this form gives:

```math
AB =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
=BA.
```

Therefore, the conditions are also sufficient. All such matrices are upper triangular with equal diagonal entries; a and b are arbitrary.
