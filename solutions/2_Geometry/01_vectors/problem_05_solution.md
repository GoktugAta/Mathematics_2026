# Exercise 5. Angle Between Vectors

## Question

Given

```math
u=(1,1,0),
\qquad
v=(1,0,1):
```

1. Use the sign of the dot product to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

## Solution

### 1. Predicting the type of angle

First, compute the dot product:

```math
u\cdot v=1(1)+1(0)+0(1)=1.
```

For nonzero vectors, the dot product satisfies

```math
u\cdot v=\|u\|\|v\|\cos\theta.
```

Since both lengths are positive, the sign of the dot product is the sign of the cosine.

Here, the dot product is positive, so the angle is less than 90 degrees. The vectors are not parallel, so the angle is also greater than zero. Therefore, we predict an acute angle.

### 2. Computing the angle

The vector lengths are

```math
\|u\|=\sqrt{1^2+1^2+0^2}=\sqrt2,
```

```math
\|v\|=\sqrt{1^2+0^2+1^2}=\sqrt2.
```

Using the angle formula gives

```math
\cos\theta
=\frac{u\cdot v}{\|u\|\|v\|}
=\frac{1}{\sqrt2\sqrt2}
=\frac12.
```

Therefore,

```math
\boxed{\theta=\arccos\left(\frac12\right)=60^\circ=\frac{\pi}{3}}.
```

### 3. Comparing with the prediction

The computed angle is 60 degrees, which lies between 0 and 90 degrees. It is acute, agreeing with our prediction from the positive dot product.
