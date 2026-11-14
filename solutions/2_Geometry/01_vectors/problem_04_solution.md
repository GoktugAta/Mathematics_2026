# Exercise 4. Dot Product and Perpendicularity

## Question

For

```math
u=(1,2,-1),
\qquad
v=(2,-1,3),
```

compute the dot product and determine whether the vectors are perpendicular.

Then find a so that

```math
w=(2,-1,a)
```

is perpendicular to u, and check the result.

## Solution

### 1. Computing the dot product

The dot product is found by multiplying corresponding components and adding the results:

```math
u\cdot v
=1(2)+2(-1)+(-1)(3).
```

Therefore,

```math
u\cdot v=2-2-3=\boxed{-3}.
```

Two nonzero vectors are perpendicular if and only if their dot product is zero.

Since the dot product is -3, u and v are not perpendicular.

### 2. Finding a for perpendicularity

For w to be perpendicular to u, we require

```math
u\cdot w=0.
```

Substituting the components gives

```math
1(2)+2(-1)+(-1)a=0.
```

Simplifying:

```math
2-2-a=0,
```

so

```math
\boxed{a=0}.
```

Thus, the required vector is

```math
w=(2,-1,0).
```

### 3. Checking the result

Using a=0, we obtain

```math
u\cdot w
=1(2)+2(-1)+(-1)(0)
=2-2+0
=0.
```

Both vectors are nonzero and their dot product is zero. Therefore, w is perpendicular to u, as required.
