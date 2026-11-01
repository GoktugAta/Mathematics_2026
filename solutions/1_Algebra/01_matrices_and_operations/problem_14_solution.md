# Problem 14 Solution

### 1. Computing R(α)R(β)

```math
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}
```

Multiplying rows by columns gives:

```math
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
```

### 2. Applying the Angle-Sum Formulas

The angle-sum identities are:

```math
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
```

```math
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
```

Substituting these identities into the product:

```math
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
=
R(\alpha+\beta)
```

### 3. Geometric Explanation

In the product R(α)R(β), the rightmost matrix acts first. A vector is first rotated through angle β about the origin, then through angle α about the same origin.

The total rotation angle is α + β. Therefore, the two successive rotations are equivalent to a single rotation through angle α + β:

```math
R(\alpha)R(\beta)=R(\alpha+\beta).
```
