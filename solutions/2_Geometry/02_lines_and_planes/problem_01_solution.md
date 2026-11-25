# Exercise 1. Line Through Two Points

## Question

Find the equation of the line through A=(1,2) and B=(4,-1) in parametric and general form.

Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

## Solution

### 1. Finding a direction vector

Subtract the coordinates of A from those of B:

```math
d=B-A=(4-1,-1-2)=(3,-3).
```

Thus, a direction vector is

```math
\boxed{d=(3,-3)}.
```

### 2. Writing the parametric form

A line through A with direction d has the form

```math
(x,y)=A+td,
\qquad t\in\mathbb{R}.
```

Therefore,

```math
\boxed{(x,y)=(1,2)+t(3,-3),\qquad t\in\mathbb{R}}.
```

Equivalently,

```math
\begin{cases}
x=1+3t,\\
y=2-3t.
\end{cases}
```

### 3. Finding a normal vector and the general form

A normal vector is perpendicular to the direction vector. Choose

```math
n=(1,1).
```

Indeed,

```math
n\cdot d=1(3)+1(-3)=0.
```

Using the point A, the normal-vector equation is

```math
n\cdot((x,y)-A)=0.
```

Thus,

```math
(x-1)+(y-2)=0.
```

The general form is

```math
\boxed{x+y-3=0}.
```

### 4. Checking both points

For A=(1,2):

```math
1+2-3=0.
```

For B=(4,-1):

```math
4+(-1)-3=0.
```

Both points satisfy the general equation.

In the parametric form, t=0 gives A, while t=1 gives B:

```math
(1,2)+0(3,-3)=(1,2),
```

```math
(1,2)+1(3,-3)=(4,-1).
```

Therefore, both forms describe the required line.
