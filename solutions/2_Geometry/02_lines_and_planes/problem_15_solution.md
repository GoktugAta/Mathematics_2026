# Exercise 15. Complete Classification of a Line Relative to a Plane

## Question

Let

```math
L:\ x=p+tv,
\qquad t\in\mathbb{R},
```

and

```math
\Pi:\ n\cdot x=d.
```

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane.

Then illustrate each case with your own simple numerical example.

## Solution

### 1. Deriving the classification

Assume v is nonzero so that L is a line, and n is nonzero so that the equation defines a plane.

A point on the line belongs to the plane precisely when

```math
n\cdot(p+tv)=d.
```

By the distributive property of the dot product,

```math
n\cdot p+t(n\cdot v)=d.
```

Therefore,

```math
t(n\cdot v)=d-n\cdot p.
```

The number of solutions for t determines the relative position.

### 2. Case 1: Exactly one intersection point

If

```math
\boxed{n\cdot v\neq0},
```

we can divide by this nonzero quantity:

```math
t_0=\frac{d-n\cdot p}{n\cdot v}.
```

There is exactly one parameter value, giving the intersection point

```math
\boxed{I=p+\frac{d-n\cdot p}{n\cdot v}v}.
```

For example, consider

```math
L:\ (x,y,z)=(0,0,1)+t(1,0,-1),
\qquad
\Pi:\ z=0.
```

Here,

```math
n=(0,0,1),
\qquad
n\cdot v=-1\neq0.
```

The plane condition is

```math
1-t=0,
```

so t=1 and the unique intersection point is

```math
\boxed{I=(1,0,0)}.
```

### 3. Case 2: Parallel with no common points

If

```math
\boxed{n\cdot v=0
\quad\text{and}\quad
n\cdot p\neq d},
```

the line's direction is parallel to the plane, but its starting point is outside the plane.

The intersection condition reduces to the false statement

```math
n\cdot p=d.
```

Therefore, no parameter value gives an intersection.

For example, consider

```math
L:\ (x,y,z)=(0,0,1)+t(1,0,0),
\qquad
\Pi:\ z=0.
```

Here,

```math
n\cdot v=0,
\qquad
n\cdot p=1\neq0.
```

Every point on the line has z=1. Thus, the line is parallel to the plane and has no common points with it.

### 4. Case 3: The line is contained in the plane

If

```math
\boxed{n\cdot v=0
\quad\text{and}\quad
n\cdot p=d},
```

the line's direction is parallel to the plane and its starting point belongs to the plane.

For every real t,

```math
n\cdot(p+tv)
=n\cdot p+t(n\cdot v)
=d+t(0)
=d.
```

Therefore, every point on the line lies in the plane.

For example, consider

```math
L:\ (x,y,z)=(0,1,0)+t(1,0,0),
\qquad
\Pi:\ z=0.
```

Here,

```math
n\cdot v=0,
\qquad
n\cdot p=0=d.
```

Every point on the line has coordinates (t,1,0), which satisfy the plane equation. Thus, the entire line is contained in the plane.

### 5. Classification summary

| Condition | Relative position | Common points |
|---|---|---|
| n·v is nonzero | The line intersects the plane once | Exactly one |
| n·v = 0 and n·p differs from d | The line is parallel and outside the plane | None |
| n·v = 0 and n·p = d | The line is contained in the plane | Infinitely many |

These cases are exhaustive because the intersection condition is a linear equation in the single parameter t.
