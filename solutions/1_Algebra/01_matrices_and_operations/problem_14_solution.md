# Exercise 14. Rotation Matrices

## Question

The matrix for a rotation through an angle θ is:

```math
R(\theta) =
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}.
```

Compute R(α)R(β) and, using the angle-sum formulas for sine and cosine, show that:

```math
R(\alpha)R(\beta)=R(\alpha+\beta).
```

Explain the result geometrically.

## Solution

### 1. Multiplying the Rotation Matrices

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}.
```

Multiplying rows by columns gives:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}.
```

### 2. Using the Angle-Sum Formulas

The angle-sum identities are:

```math
\cos(\alpha+\beta)
=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
```

```math
\sin(\alpha+\beta)
=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
```

Substituting these identities gives:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
=R(\alpha+\beta).
```

### 3. Geometric Explanation

The rightmost matrix acts first. Thus, R(α)R(β) first rotates a vector through β and then through α, both about the origin.

The total rotation angle is α + β, so these two rotations are equivalent to one rotation through α + β.
