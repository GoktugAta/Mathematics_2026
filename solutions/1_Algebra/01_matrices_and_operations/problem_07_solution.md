# Problem 7 Solution

### 1. Computations ($AI$, $IA$, $A + 0$, $A^2$, $A^3$)

$$
AI =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
$$

$$
IA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
$$

$$
A + 0 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} +
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix} =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
$$

$$
A^2 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
$$

$$
A^3 = A^2 A =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} =
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}
$$

### 2. Roles of $I$ and $0$

* **Identity Matrix ($I$):** Acts as the multiplicative identity, meaning multiplying any matrix by $I$ leaves the matrix unchanged ($AI = IA = A$).
* **Zero Matrix ($0$):** Acts as the additive identity, meaning adding the zero matrix to $A$ leaves $A$ unchanged ($A + 0 = A$).

### 3. Pattern in Successive Powers of $A$

For $A = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$, the powers follow the pattern:

$$
A^n =
\begin{pmatrix}
2^n & n \cdot 2^{n-1} \\
0 & 2^n
\end{pmatrix}
$$
