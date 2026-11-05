# Exercise 13. A Recurrence Written in Matrix Form

## Question

Let

```math
F =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}.
```

Compute F², F³, F⁴, and F⁵. Compare the numbers obtained with the sequence

```math
0,1,1,2,3,5,8,\ldots
```

and describe the relationship you observe. Then compute

```math
F\begin{pmatrix}
a \\
b
\end{pmatrix}
```

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

### 1. Computing the Powers

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
\end{pmatrix}.
```

```math
F^3 =
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
\end{pmatrix}.
```

```math
F^4 =
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
\end{pmatrix}.
```

```math
F^5 =
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
\end{pmatrix}.
```

### 2. Relationship with Fibonacci Numbers

The entries are consecutive Fibonacci numbers. Define:

```math
f_0=0,\qquad f_1=1,
\qquad f_{n+1}=f_n+f_{n-1}\quad(n\geq1).
```

The pattern is:

```math
F^n =
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1}
\end{pmatrix},
\qquad n\geq1.
```

Multiplication by F advances the entries to the next Fibonacci numbers.

### 3. One Recurrence Step

```math
F\begin{pmatrix}
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
\end{pmatrix}.
```

If a is the current term and b is the previous term, the new first entry a + b is the next term. The second entry keeps a as the previous term for the following step.

In particular:

```math
F\begin{pmatrix}
f_{n+1} \\
f_n
\end{pmatrix}
=
\begin{pmatrix}
f_{n+2} \\
f_{n+1}
\end{pmatrix}.
```

Thus, multiplication by F performs one step of the Fibonacci recurrence.
