# Exercise 8. Sphere

## Question

Reduce

```math
x^2+y^2+z^2-4x+2y-6z-2=0
```

to canonical form. Find the center and radius.

Give two points on the sphere and check them in the equation.

## Solution

### 1. Grouping the terms

Move the constant to the right and group terms by coordinate:

```math
(x^2-4x)+(y^2+2y)+(z^2-6z)=2.
```

### 2. Completing the squares

Use the identities

```math
x^2-4x=(x-2)^2-4,
```

```math
y^2+2y=(y+1)^2-1,
```

```math
z^2-6z=(z-3)^2-9.
```

Substituting gives

```math
(x-2)^2-4+(y+1)^2-1+(z-3)^2-9=2.
```

Therefore, the canonical form is

```math
\boxed{(x-2)^2+(y+1)^2+(z-3)^2=16}.
```

### 3. Finding the center and radius

Compare with the standard sphere equation:

```math
(x-h)^2+(y-k)^2+(z-l)^2=r^2.
```

Thus,

```math
\boxed{C=(2,-1,3),\qquad r=4}.
```

### 4. Choosing two points

Move four units from the center in each direction along the x-axis:

```math
A=(6,-1,3),
\qquad
B=(-2,-1,3).
```

### 5. Checking A

In canonical form:

```math
(6-2)^2+(-1+1)^2+(3-3)^2=16.
```

In the original equation:

```math
6^2+(-1)^2+3^2-4(6)+2(-1)-6(3)-2
=36+1+9-24-2-18-2
=0.
```

Therefore, A lies on the sphere.

### 6. Checking B

In canonical form:

```math
(-2-2)^2+(-1+1)^2+(3-3)^2=16.
```

In the original equation:

```math
(-2)^2+(-1)^2+3^2-4(-2)+2(-1)-6(3)-2
=4+1+9+8-2-18-2
=0.
```

Therefore, B also lies on the sphere. Both points satisfy the original and canonical equations.
