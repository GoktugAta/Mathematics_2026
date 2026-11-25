# Exercise 14. Closest Point on a Line

## Question

Given a point P=(4,1) and a line through the origin with direction v=(1,2), use projection to find the closest point on the line and the distance from P to the line.

Verify that the appropriate vector is perpendicular to the direction of the line.

## Solution

### 1. Finding the closest point by projection

The line consists of points of the form

```math
Q=tv=t(1,2),
\qquad t\in\mathbb{R}.
```

Since the line passes through the origin, the closest point is the projection of the position vector p=(4,1) onto v:

```math
q=\frac{p\cdot v}{v\cdot v}v.
```

The dot products are

```math
p\cdot v=4(1)+1(2)=6,
```

```math
v\cdot v=1^2+2^2=5.
```

Therefore,

```math
q=\frac65(1,2)
=\left(\frac65,\frac{12}{5}\right).
```

Thus, the closest point is

```math
\boxed{Q=\left(\frac65,\frac{12}{5}\right)}.
```

It lies on the line because its position vector is a scalar multiple of v.

### 2. Finding the perpendicular displacement

The vector from Q to P is

```math
\overrightarrow{QP}=P-Q.
```

Therefore,

```math
\overrightarrow{QP}
=\left(4-\frac65,1-\frac{12}{5}\right)
=\left(\frac{14}{5},-\frac75\right).
```

### 3. Computing the distance

The distance from P to the line is the length of this perpendicular displacement:

```math
d=\left\|\overrightarrow{QP}\right\|
=\sqrt{\left(\frac{14}{5}\right)^2+
\left(-\frac75\right)^2}.
```

Hence,

```math
d=\sqrt{\frac{196+49}{25}}
=\frac{\sqrt{245}}5
=\boxed{\frac{7\sqrt5}{5}}.
```

### 4. Checking perpendicularity

Compute the dot product with the line direction:

```math
\overrightarrow{QP}\cdot v
=\left(\frac{14}{5},-\frac75\right)\cdot(1,2)
=\frac{14}{5}-\frac{14}{5}
=0.
```

Thus, the vector from Q to P is perpendicular to the line.

### 5. Why this point is the closest

For any other point R on the line, Q-R is parallel to v and perpendicular to P-Q. Therefore, the Pythagorean theorem gives

```math
\|P-R\|^2=\|P-Q\|^2+\|Q-R\|^2.
```

The second term is nonnegative, so

```math
\|P-R\|\geq\|P-Q\|.
```

Equality holds only when R=Q. Therefore, Q is the unique closest point on the line.
