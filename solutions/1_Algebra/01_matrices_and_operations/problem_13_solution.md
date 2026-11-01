# Problem 13 Solution

### 1. Computing F²

```math
F^2 =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
```

### 2. Computing F³

```math
F^3 = F^2 F =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
```

### 3. Computing F⁴

```math
F^4 = F^3 F =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
```

### 4. Computing F⁵

```math
F^5 = F^4 F =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
```

### 5. Relationship with the Fibonacci Sequence

The entries are consecutive Fibonacci numbers. Define:

```math
f_0 = 0,
\qquad
f_1 = 1,
\qquad
f_{n+1} = f_n + f_{n-1}
\quad (n \geq 1).
```

The observed pattern is:

```math
F^n =
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1}
\end{pmatrix}
\quad (n \geq 1).
```

Multiplying this matrix by F gives:

```math
F^{n+1} =
\begin{pmatrix}
f_{n+1}+f_n & f_{n+1} \\
f_n+f_{n-1} & f_n
\end{pmatrix}
=
\begin{pmatrix}
f_{n+2} & f_{n+1} \\
f_{n+1} & f_n
\end{pmatrix}.
```

Thus, each multiplication advances the Fibonacci pattern by one step.

### 6. Multiplying F by a Column Vector

```math
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
```

If a is the current term and b is the previous term, the new first entry is the next term, a + b. The second entry keeps a for the following step.

For Fibonacci numbers:

```math
F
\begin{pmatrix}
f_{n+1} \\
f_n
\end{pmatrix}
=
\begin{pmatrix}
f_{n+2} \\
f_{n+1}
\end{pmatrix}.
```

Therefore, multiplication by F performs one step of the Fibonacci recurrence.
