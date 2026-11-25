# Exercise 15. Comparing Directions Using the Cosine of the Angle

## Question

Given

```math
a=(1,2,1),
\qquad
b=(2,4,2),
\qquad
c=(2,0,3),
```

for each pair compute

```math
\frac{u\cdot v}{\|u\|\|v\|}.
```

Order the pairs by increasing angle between the vectors. Explain why for a and b the value is 1 even though the vectors have different lengths.

## Solution

### 1. Computing the vector lengths

The required lengths are

```math
\|a\|=\sqrt{1^2+2^2+1^2}=\sqrt6,
```

```math
\|b\|=\sqrt{2^2+4^2+2^2}=\sqrt{24}=2\sqrt6,
```

```math
\|c\|=\sqrt{2^2+0^2+3^2}=\sqrt{13}.
```

For nonzero vectors, the given expression equals the cosine of their angle:

```math
\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}.
```

### 2. Comparing a and b

Their dot product is

```math
a\cdot b=1(2)+2(4)+1(2)=12.
```

Therefore,

```math
\cos\theta_{ab}
=\frac{12}{\sqrt6(2\sqrt6)}
=\frac{12}{12}
=\boxed{1}.
```

Thus,

```math
\boxed{\theta_{ab}=0^\circ}.
```

### 3. Comparing a and c

Their dot product is

```math
a\cdot c=1(2)+2(0)+1(3)=5.
```

Therefore,

```math
\boxed{\cos\theta_{ac}=\frac{5}{\sqrt{78}}}.
```

The angle is

```math
\theta_{ac}=\arccos\left(\frac5{\sqrt{78}}\right).
```

It is acute because its cosine is strictly between zero and one.

### 4. Comparing b and c

Their dot product is

```math
b\cdot c=2(2)+4(0)+2(3)=10.
```

Therefore,

```math
\cos\theta_{bc}
=\frac{10}{2\sqrt6\sqrt{13}}
=\boxed{\frac5{\sqrt{78}}}.
```

Hence,

```math
\theta_{bc}=\arccos\left(\frac5{\sqrt{78}}\right)
=\theta_{ac}.
```

### 5. Ordering the pairs by increasing angle

Cosine decreases as the angle increases from 0 to 180 degrees. Since

```math
1>\frac5{\sqrt{78}}>0,
```

the order is

```math
\boxed{\theta_{ab}<\theta_{ac}=\theta_{bc}}.
```

The pair (a,b) has the smallest angle, while (a,c) and (b,c) have equal angles.

### 6. Why a and b have cosine 1

We have

```math
b=2a.
```

Since the multiplier is positive, a and b have the same direction and orientation. Their lengths differ, but the angle between them is zero.

The normalization in the cosine formula cancels the length factor:

```math
\frac{a\cdot(2a)}{\|a\|\|2a\|}
=\frac{2\|a\|^2}{2\|a\|^2}
=1.
```

Therefore, the expression compares direction independently of length. This also explains why a and b make the same angle with c.
