# Exercise 9. Ellipsoid and Its Cross-Sections

## Question

Consider

```math
\frac{x^2}{9}+\frac{y^2}{4}+\frac{z^2}{16}=1.
```

Give the semiaxis lengths, describe the cross-section z=0, and explain how the cross-sections z=c change for |c|<4.

## Solution

### 1. Identifying the semiaxis lengths

The standard equation of an ellipsoid centered at the origin is

```math
\frac{x^2}{a^2}+\frac{y^2}{b^2}+\frac{z^2}{d^2}=1.
```

Taking square roots of the denominators gives the semiaxis lengths:

```math
\boxed{3\text{ along }x,\qquad
2\text{ along }y,\qquad
4\text{ along }z}.
```

Thus, the ellipsoid is longest along the z-axis. Its axis intercepts are

```math
(\pm3,0,0),\qquad
(0,\pm2,0),\qquad
(0,0,\pm4).
```

### 2. Describing the cross-section z=0

Substituting z=0 gives

```math
\frac{x^2}{9}+\frac{y^2}{4}=1.
```

This is an ellipse in the xy-plane, centered at the origin, with semiaxis lengths 3 and 2.

### 3. Describing the cross-sections z=c

Substituting z=c gives

```math
\frac{x^2}{9}+\frac{y^2}{4}
=1-\frac{c^2}{16}.
```

For |c|<4, the right-hand side is positive. Dividing by it gives

```math
\frac{x^2}{9\left(1-\frac{c^2}{16}\right)}
+
\frac{y^2}{4\left(1-\frac{c^2}{16}\right)}
=1.
```

Therefore, the cross-section is an ellipse in the plane z=c, centered at (0,0,c), with semiaxis lengths

```math
\boxed{
a_c=3\sqrt{1-\frac{c^2}{16}},
\qquad
b_c=2\sqrt{1-\frac{c^2}{16}}
}.
```

### 4. Explaining how the sections change

The largest horizontal section occurs at c=0.

As |c| increases toward 4, both semiaxis lengths decrease toward zero. Their ratio remains

```math
\frac{a_c}{b_c}=\frac32,
```

so the ellipses keep the same proportions while becoming smaller.

The sections at c and -c have the same size because the formulas depend on c^2.

At c=±4, the section reduces to the single point (0,0,±4). For |c|>4, there are no real points because the sum of the nonnegative x and y terms would have to be negative.
