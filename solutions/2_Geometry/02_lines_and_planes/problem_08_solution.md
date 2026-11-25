# Exercise 8. Intersection Point of a Line and a Plane

## Question

Find the intersection point of the line

```math
(x,y,z)=(1,0,2)+t(1,2,-1),
\qquad t\in\mathbb{R},
```

with the plane

```math
x+y+z=4.
```

Check the result by substituting it into both descriptions.

## Solution

### 1. Substituting the line into the plane equation

The coordinate equations of the line are

```math
x=1+t,
\qquad
y=2t,
\qquad
z=2-t.
```

At the intersection, these coordinates must satisfy the plane equation:

```math
(1+t)+2t+(2-t)=4.
```

Simplifying gives

```math
3+2t=4,
\qquad
t=\frac12.
```

This is the unique parameter value satisfying the equation, so there is exactly one intersection point.

### 2. Finding the intersection point

Substitute t=1/2 into the line:

```math
x=1+\frac12=\frac32,
```

```math
y=2\left(\frac12\right)=1,
```

```math
z=2-\frac12=\frac32.
```

Therefore, the intersection point is

```math
\boxed{I=\left(\frac32,1,\frac32\right)}.
```

### 3. Checking the line description

Using t=1/2 gives

```math
(1,0,2)+\frac12(1,2,-1)
=\left(\frac32,1,\frac32\right)=I.
```

Thus, I lies on the line.

### 4. Checking the plane equation

Substituting I gives

```math
\frac32+1+\frac32=4.
```

Thus, I also lies in the plane, confirming the intersection.
