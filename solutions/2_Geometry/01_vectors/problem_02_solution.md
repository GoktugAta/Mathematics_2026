# Exercise 2. Distance as the Length of a Vector

## Question

The points are A=(1,2,3) and B=(4,-2,6).

1. Construct the vector from A to B.
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

## Solution

### 1. Constructing the displacement vector

To find the vector from A to B, subtract the coordinates of the starting point A from those of the endpoint B:

```math
\overrightarrow{AB}=B-A.
```

Therefore,

```math
\overrightarrow{AB}
=(4-1,-2-2,6-3)
=\boxed{(3,-4,3)}.
```

This vector describes the displacement from A to B. We can check its endpoint:

```math
A+\overrightarrow{AB}
=(1,2,3)+(3,-4,3)
=(4,-2,6)=B.
```

### 2. Computing the vector length

The Euclidean length of a vector is the square root of the sum of the squares of its components:

```math
\left\|\overrightarrow{AB}\right\|
=\sqrt{3^2+(-4)^2+3^2}
=\sqrt{9+16+9}.
```

Thus,

```math
\boxed{\left\|\overrightarrow{AB}\right\|=\sqrt{34}}.
```

### 3. Computing the distance using coordinates

The distance formula in three-dimensional space is

```math
d(A,B)=
\sqrt{(x_B-x_A)^2+(y_B-y_A)^2+(z_B-z_A)^2}.
```

Substituting the coordinates gives

```math
d(A,B)
=\sqrt{(4-1)^2+(-2-2)^2+(6-3)^2}
=\sqrt{9+16+9}.
```

Therefore,

```math
\boxed{d(A,B)=\sqrt{34}}.
```

### 4. Explaining why the results agree

The distance between two points is the length of the displacement vector joining them:

```math
d(A,B)=\left\|B-A\right\|
=\left\|\overrightarrow{AB}\right\|.
```

The coordinate distance formula uses exactly the same coordinate differences as the vector-length calculation. Both formulas follow from the Pythagorean theorem, so they give the same result.
