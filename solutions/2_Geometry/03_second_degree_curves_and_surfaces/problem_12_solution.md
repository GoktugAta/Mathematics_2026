# Exercise 12. Recognizing a Surface from Cross-Sections

## Question

A certain surface has the following properties:

- The cross-section z=0 is a point.
- For z>0, the cross-sections z=constant are circles with increasing radius.
- Vertical cross-sections through the Oz axis are parabolas.

Propose a simple equation for such a surface and justify your choice.

## Solution

### 1. Proposing an equation

A suitable equation is

```math
\boxed{z=x^2+y^2}.
```

This describes a circular paraboloid opening in the positive z-direction.

### 2. Checking the section z=0

Substituting z=0 gives

```math
x^2+y^2=0.
```

Since both squares are nonnegative, this requires

```math
x=0,\qquad y=0.
```

Therefore, the section consists of the single point

```math
(0,0,0).
```

### 3. Checking the horizontal sections for z>0

For a fixed height z=c>0, the equation becomes

```math
x^2+y^2=c.
```

This is a circle in the plane z=c, centered at (0,0,c), with radius

```math
r=\sqrt c.
```

As c increases, the radius increases. This matches the second property.

### 4. Checking vertical sections through the z-axis

Any vertical plane through the z-axis can be parametrized by

```math
x=s\cos\theta,
\qquad
y=s\sin\theta,
```

where θ is fixed, s is a signed horizontal coordinate, and z is unrestricted.

Substituting into the surface equation gives

```math
z=s^2\cos^2\theta+s^2\sin^2\theta.
```

Using the identity cos²θ+sin²θ=1, we obtain

```math
z=s^2.
```

This is an upward-opening parabola in that vertical plane.

Therefore, every vertical cross-section through the z-axis is a parabola, and the proposed equation satisfies all three properties.
