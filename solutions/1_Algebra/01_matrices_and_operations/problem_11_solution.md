# Problem 11 Solution

### 1. Computing AB

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
\end{pmatrix}
```

### 2. Computing BA

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
\end{pmatrix}
```

### 3. Conditions for AB = BA

Corresponding entries must be equal:

```math
\begin{cases}
a+c = a, \\
b+d = a+b, \\
c = c, \\
d = c+d.
\end{cases}
```

The first and fourth equations give c = 0. The second gives d = a. The third imposes no additional condition.

Therefore, the necessary and sufficient conditions are:

```math
c = 0,
\qquad
d = a.
```

There are no restrictions on a or b.

### 4. General Form of B

All matrices commuting with A have the form:

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix},
\qquad
a,b \in \mathbb{R}.
```

To verify sufficiency, substitute this form:

```math
AB =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
= BA.
```

Thus, B commutes with A exactly when B is upper triangular with equal diagonal entries.
