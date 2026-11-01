# Problem 4 Solution

### 1. Computing AB

$$
AB = 
\left(\begin{array}{cc}
1 & 2 \\
0 & 1
\end{array}\right)
\left(\begin{array}{cc}
2 & 0 \\
3 & 1
\end{array}\right)
=
\left(\begin{array}{cc}
8 & 2 \\
3 & 1
\end{array}\right)
$$

### 2. Computing BA

$$
BA = 
\left(\begin{array}{cc}
2 & 0 \\
3 & 1
\end{array}\right)
\left(\begin{array}{cc}
1 & 2 \\
0 & 1
\end{array}\right)
=
\left(\begin{array}{cc}
2 & 4 \\
3 & 7
\end{array}\right)
$$

### 3. Is AB = BA?

No, $AB \neq BA$ because:

$$
\left(\begin{array}{cc}
8 & 2 \\
3 & 1
\end{array}\right)
\neq
\left(\begin{array}{cc}
2 & 4 \\
3 & 7
\end{array}\right)
$$

### 4. Explanation of Noncommutativity

Matrix multiplication is generally **noncommutative**, meaning that changing the order of multiplication ($AB$ versus $BA$) does not yield the same result. This is a fundamental difference from ordinary number multiplication where $ab = ba$ is always true.
