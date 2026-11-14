# Exercise 8. Linear Combination and Checking the Result

## Question

Check whether w=(5,1) can be written as

```math
w=au+bv,
```

where u=(1,1) and v=(2,-1).

If so, find a and b, reconstruct w from them, and explain the geometric meaning of the existence of such coefficients.

## Solution

### 1. Forming a system for the coefficients

Substituting the vectors into w=au+bv gives

```math
(5,1)=a(1,1)+b(2,-1).
```

The right-hand side is

```math
a(1,1)+b(2,-1)=(a+2b,a-b).
```

Equating corresponding components gives

```math
\begin{cases}
a+2b=5,\\
a-b=1.
\end{cases}
```

### 2. Solving for a and b

Subtract the second equation from the first:

```math
(a+2b)-(a-b)=5-1.
```

Therefore,

```math
3b=4,
\qquad
b=\frac43.
```

Using a-b=1 gives

```math
a=1+b=1+\frac43=\frac73.
```

Thus,

```math
\boxed{a=\frac73,\qquad b=\frac43}.
```

### 3. Reconstructing w

Substitute the coefficients back into the linear combination:

```math
au+bv
=\frac73(1,1)+\frac43(2,-1).
```

Therefore,

```math
au+bv
=\left(\frac73,\frac73\right)
+\left(\frac83,-\frac43\right)
=\left(\frac{15}{3},\frac33\right)
=(5,1)=w.
```

This confirms that the coefficients are correct.

### 4. Geometric meaning

The existence of these coefficients means that w belongs to the span of u and v. We can obtain the displacement w by scaling u and v and then adding them using the head-to-tail rule.

The vectors u and v are not parallel: if v were a multiple of u, its two components would be equal, but 2 and -1 are different.

Two nonparallel vectors in the plane span the entire plane. Therefore, every vector in the plane can be expressed as a linear combination of u and v, and the coefficients are unique.
