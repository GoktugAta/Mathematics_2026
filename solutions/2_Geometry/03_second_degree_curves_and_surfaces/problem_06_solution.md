# Exercise 6. Shifted Ellipse

## Question

Reduce

```math
4x^2+9y^2-16x+18y-11=0
```

to canonical form. Give the center and semiaxis lengths.

Check that substituting the coordinates of the center into the left-hand side gives a value consistent with the form you obtained.

## Solution

### 1. Completing the squares

Group the terms and factor out the quadratic coefficients:

```math
4(x^2-4x)+9(y^2+2y)-11=0.
```

Use the identities

```math
x^2-4x=(x-2)^2-4,
```

```math
y^2+2y=(y+1)^2-1.
```

Substituting gives

```math
4(x-2)^2-16+9(y+1)^2-9-11=0.
```

Therefore,

```math
4(x-2)^2+9(y+1)^2=36.
```

Dividing by 36 gives the canonical form:

```math
\boxed{\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1}.
```

### 2. Identifying the center and semiaxes

The center is read from the coordinate shifts:

```math
\boxed{C=(2,-1)}.
```

The semiaxis lengths are the square roots of the denominators:

```math
\boxed{a=3,\qquad b=2}.
```

The horizontal semiaxis has length 3, and the vertical semiaxis has length 2. Thus, the major axis is horizontal.

### 3. Checking the value at the center

Let the original left-hand side be

```math
F(x,y)=4x^2+9y^2-16x+18y-11.
```

At C=(2,-1):

```math
F(2,-1)
=4(2)^2+9(-1)^2-16(2)+18(-1)-11.
```

Hence,

```math
F(2,-1)=16+9-32-18-11=-36.
```

This agrees with the completed-square expression:

```math
F(x,y)=4(x-2)^2+9(y+1)^2-36.
```

At the center, both squared terms vanish, leaving -36.

The center is inside the ellipse, not on the curve. Therefore, its substitution should not give zero. In the normalized canonical form, the left-hand side at the center is 0, whereas points on the ellipse have value 1.
