# Exercise 11. Decomposition into Parallel and Perpendicular Components

## Question

Decompose u=(3,4) into components parallel and perpendicular to v=(1,2).

Check that

```math
u=u_{\parallel}+u_{\perp},
\qquad
u_{\perp}\cdot v=0.
```

Explain why these are two independent checks of correctness.

## Solution

### 1. Finding the parallel component

The component parallel to v is the projection of u onto v:

```math
u_{\parallel}=\frac{u\cdot v}{v\cdot v}v.
```

The required dot products are

```math
u\cdot v=3(1)+4(2)=11,
```

```math
v\cdot v=1^2+2^2=5.
```

Therefore,

```math
u_{\parallel}
=\frac{11}{5}(1,2)
=\boxed{\left(\frac{11}{5},\frac{22}{5}\right)}.
```

This vector is parallel to v because it is a scalar multiple of v.

### 2. Finding the perpendicular component

Subtract the parallel component from u:

```math
u_{\perp}=u-u_{\parallel}.
```

Thus,

```math
u_{\perp}
=(3,4)-\left(\frac{11}{5},\frac{22}{5}\right)
=\boxed{\left(\frac45,-\frac25\right)}.
```

### 3. Checking reconstruction

Adding the two components gives

```math
u_{\parallel}+u_{\perp}
=
\left(\frac{11}{5}+\frac45,
\frac{22}{5}-\frac25\right)
=
\left(\frac{15}{5},\frac{20}{5}\right)
=(3,4)=u.
```

Therefore, the components reconstruct the original vector.

### 4. Checking perpendicularity

Compute the dot product with v:

```math
u_{\perp}\cdot v
=\left(\frac45,-\frac25\right)\cdot(1,2)
=\frac45-\frac45
=0.
```

Therefore, the perpendicular component is orthogonal to v.

### 5. Why both checks are needed

The reconstruction check confirms that the components add up to u. However, many pairs of vectors add up to u without having the required directions.

The perpendicularity check confirms that the remainder is orthogonal to v. By itself, this does not confirm that the two components add up to u.

Thus, the checks test different requirements. Together with the fact that the parallel component is a scalar multiple of v, they verify the required decomposition.
