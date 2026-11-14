# Exercise 1. Vector Operations and Their Meaning

## Question

For

```math
u=(2,-1,3),
\qquad
v=(-1,4,2),
```

compute

```math
u+v,\qquad u-v,\qquad 3u-2v.
```

Then verify that

```math
(u+v)-v=u,
```

and explain geometrically what adding two vectors means.

## Solution

### 1. Computing u + v

Vector addition is performed by adding corresponding components:

```math
u+v=(2+(-1),-1+4,3+2).
```

Therefore,

```math
\boxed{u+v=(1,3,5)}.
```

### 2. Computing u - v

We subtract each component of v from the corresponding component of u:

```math
u-v=(2-(-1),-1-4,3-2).
```

Subtracting a negative number gives addition, so

```math
\boxed{u-v=(3,-5,1)}.
```

### 3. Computing 3u - 2v

First, multiply every component by the appropriate scalar:

```math
3u=(6,-3,9),
```

```math
2v=(-2,8,4).
```

Then subtract corresponding components:

```math
3u-2v=(6-(-2),-3-8,9-4).
```

Thus,

```math
\boxed{3u-2v=(8,-11,5)}.
```

### 4. Verifying the identity

Using u+v=(1,3,5), we obtain

```math
(u+v)-v=(1,3,5)-(-1,4,2).
```

Therefore,

```math
(u+v)-v=(1-(-1),3-4,5-2)
=(2,-1,3)=u.
```

This verifies the identity. Adding v and then subtracting v cancels its effect and returns the original vector.

### 5. Geometric meaning of vector addition

A vector represents a displacement with a magnitude and a direction.

To add u and v geometrically, draw u first. Then place the tail of v at the head of u without changing its length or direction. The sum u+v runs from the starting point of u to the final endpoint of v. This is the head-to-tail rule.

In this example, starting at the origin and moving by u brings us to

```math
(2,-1,3).
```

Moving from this point by v brings us to

```math
(2-1,-1+4,3+2)=(1,3,5).
```

Therefore, the total displacement is

```math
u+v=(1,3,5).
```

Equivalently, if u and v are drawn from the same starting point, their sum is the diagonal of the parallelogram formed by the two vectors.
