# Exercise 3. Vector Normalization

## Question

For v=(3,4), find a unit vector e with the same direction and orientation.

Check that its length is 1, reconstruct v in the form

```math
v=\|v\|e,
```

and explain what changes during normalization and what remains unchanged.

## Solution

### 1. Computing the length of v

The length of v is

```math
\|v\|=\sqrt{3^2+4^2}
=\sqrt{9+16}
=5.
```

Since v is nonzero, we can divide it by its length.

### 2. Finding the unit vector

To normalize a nonzero vector, divide each component by its length:

```math
e=\frac{v}{\|v\|}.
```

Therefore,

```math
e=\frac{1}{5}(3,4)
=\boxed{\left(\frac35,\frac45\right)}.
```

The multiplier 1/5 is positive, so e points in the same direction and orientation as v.

### 3. Checking the length of e

Using the length formula:

```math
\|e\|
=\sqrt{\left(\frac35\right)^2+\left(\frac45\right)^2}
=\sqrt{\frac9{25}+\frac{16}{25}}
=\sqrt{1}
=1.
```

Thus, e is a unit vector.

### 4. Reconstructing v

Multiplying the unit vector by the original length gives

```math
\|v\|e
=5\left(\frac35,\frac45\right)
=(3,4)
=v.
```

Therefore,

```math
\boxed{v=5e}.
```

### 5. Meaning of normalization

Normalization changes the vector's length from 5 to 1. Its components are scaled by the same positive factor, so its direction and orientation remain unchanged.

The representation

```math
v=\|v\|e
```

separates the magnitude, given by the scalar 5, from the direction and orientation, given by the unit vector e.

The zero vector cannot be normalized because its length is zero, and division by zero is undefined.
