# Exercise 5. Relative Position of Two Lines

## Question

Analyze the position of

```math
L_1:\ (x,y,z)=(1,1,0)+t(1,2,1),
\qquad t\in\mathbb{R},
```

```math
L_2:\ (x,y,z)=(2,0,1)+s(0,1,-1),
\qquad s\in\mathbb{R}.
```

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.

## Solution

### 1. Comparing the direction vectors

The direction vectors are

```math
d_1=(1,2,1),
\qquad
d_2=(0,1,-1).
```

They are not scalar multiples: every scalar multiple of d_2 has first component zero, whereas d_1 has first component one.

Therefore, the lines are not parallel.

### 2. Checking for an intersection

An intersection requires parameter values t and s that give the same three coordinates:

```math
\begin{cases}
1+t=2,\\
1+2t=s,\\
t=1-s.
\end{cases}
```

From the first equation:

```math
t=1.
```

The second equation then gives

```math
s=1+2(1)=3.
```

However, the third equation would require

```math
1=1-3=-2,
```

which is impossible.

Therefore, there is no pair of parameter values satisfying all three equations, and the lines do not intersect.

### 3. Classification

The lines are neither parallel nor intersecting. Hence,

```math
\boxed{L_1\text{ and }L_2\text{ are skew lines}}.
```

Skew lines are nonparallel lines in three-dimensional space that do not intersect. They cannot lie in the same plane.
