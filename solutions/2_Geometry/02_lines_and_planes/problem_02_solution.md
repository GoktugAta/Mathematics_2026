# Exercise 2. A Line in Space

## Question

Given the line

```math
L:\ (x,y,z)=(2,-1,3)+t(1,2,-2),
\qquad t\in\mathbb{R},
```

state a point on the line and its direction vector, check whether P=(4,3,-1) lies on L, and find the point corresponding to t=-1.

## Solution

### 1. Identifying a point and the direction vector

The parametric form consists of a fixed point plus a scalar multiple of a direction vector.

Setting t=0 gives the point

```math
\boxed{Q=(2,-1,3)}.
```

The direction vector is

```math
\boxed{d=(1,2,-2)}.
```

The coordinate equations are

```math
\begin{cases}
x=2+t,\\
y=-1+2t,\\
z=3-2t.
\end{cases}
```

### 2. Checking whether P lies on the line

A point belongs to the line if one common parameter value satisfies all three coordinate equations.

Using the x-coordinate of P gives

```math
4=2+t,
\qquad t=2.
```

Check the other coordinates using this same value:

```math
y=-1+2(2)=3,
```

```math
z=3-2(2)=-1.
```

All coordinates agree with P. Therefore,

```math
\boxed{P\in L,\qquad t=2}.
```

### 3. Finding the point for t=-1

Substitute t=-1 into the parametric equation:

```math
(x,y,z)
=(2,-1,3)-(1,2,-2).
```

Hence,

```math
\boxed{(x,y,z)=(1,-3,5)}.
```
