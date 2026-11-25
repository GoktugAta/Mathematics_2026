# Exercise 2. Circle by Completing the Square

## Question

Reduce

```math
x^2+y^2-6x+4y-3=0
```

to canonical form.

Find the center and radius, then substitute two simple points from the circle into both forms of the equation.

## Solution

### 1. Grouping the terms

Group the x terms and the y terms, and move the constant to the right:

```math
(x^2-6x)+(y^2+4y)=3.
```

### 2. Completing the square

For the x terms, half of -6 is -3, whose square is 9:

```math
x^2-6x=(x-3)^2-9.
```

For the y terms, half of 4 is 2, whose square is 4:

```math
y^2+4y=(y+2)^2-4.
```

Substituting gives

```math
(x-3)^2-9+(y+2)^2-4=3.
```

Therefore, the canonical form is

```math
\boxed{(x-3)^2+(y+2)^2=16}.
```

### 3. Identifying the center and radius

Compare with the standard circle equation:

```math
(x-h)^2+(y-k)^2=r^2.
```

Since y+2=y-(-2), the center and radius are

```math
\boxed{C=(3,-2),\qquad r=4}.
```

### 4. Choosing two simple points

Move four units horizontally from the center in each direction:

```math
A=(7,-2),
\qquad
B=(-1,-2).
```

Both points should lie on the circle because each is four units from its center.

### 5. Checking A in both forms

In the canonical form:

```math
(7-3)^2+(-2+2)^2=16+0=16.
```

In the original form:

```math
7^2+(-2)^2-6(7)+4(-2)-3
=49+4-42-8-3
=0.
```

Thus, A satisfies both equations.

### 6. Checking B in both forms

In the canonical form:

```math
(-1-3)^2+(-2+2)^2=16+0=16.
```

In the original form:

```math
(-1)^2+(-2)^2-6(-1)+4(-2)-3
=1+4+6-8-3
=0.
```

Thus, B also satisfies both equations.

Completing the square used equivalent algebraic steps, so the original and canonical equations describe the same circle. The substitutions confirm that the two selected points satisfy both descriptions.
