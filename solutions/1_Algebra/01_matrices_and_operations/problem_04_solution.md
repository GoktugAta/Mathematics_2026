# Problem 4 Solution

### 1. Computing AB
$$
AB = \begin{pmatrix}
1 \quad 2 \newline
0 \quad 1
\end{pmatrix}
\begin{pmatrix}
2 \quad 0 \newline
3 \quad 1
\end{pmatrix}
=
\begin{pmatrix}
8 \quad 2 \newline
3 \quad 1
\end{pmatrix}
$$

### 2. Computing BA
$$
BA = \begin{pmatrix}
2 \quad 0 \newline
3 \quad 1
\end{pmatrix}
\begin{pmatrix}
1 \quad 2 \newline
0 \quad 1
\end{pmatrix}
=
\begin{pmatrix}
2 \quad 4 \newline
3 \quad 7
\end{pmatrix}
$$

### 3. Is AB = BA?
No, $AB \neq BA$ because:
$$
\begin{pmatrix}
8 \quad 2 \newline
3 \quad 1
\end{pmatrix}
\neq
\begin{pmatrix}
2 \quad 4 \newline
3 \quad 7
\end{pmatrix}
$$

### 4. Explanation of Noncommutativity
Matrix multiplication is generally **noncommutative**, meaning that changing the order of multiplication ($AB$ versus $BA$) does not yield the same result. This is a fundamental difference from ordinary number multiplication where $ab = ba$ is always true
