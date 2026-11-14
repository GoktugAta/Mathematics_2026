# Exercise 9. Cross Product as a Perpendicular Direction

## Question

For

```math
u=(1,2,0),
\qquad
v=(0,1,3),
```

compute the cross product u × v.

Use dot products to check perpendicularity to both vectors, compute v × u, and compare the results.

## Solution

### 1. Computing u × v

For three-dimensional vectors, the cross product is

```math
u\times v=
(u_2v_3-u_3v_2,\;
u_3v_1-u_1v_3,\;
u_1v_2-u_2v_1).
```

Substituting the components gives

```math
u\times v=
(2(3)-0(1),\;
0(0)-1(3),\;
1(1)-2(0)).
```

Therefore,

```math
\boxed{u\times v=(6,-3,1)}.
```

### 2. Checking perpendicularity to u

Compute the dot product:

```math
(u\times v)\cdot u
=(6,-3,1)\cdot(1,2,0).
```

Thus,

```math
(u\times v)\cdot u
=6(1)+(-3)(2)+1(0)
=6-6
=0.
```

Since the vectors are nonzero, this confirms that u × v is perpendicular to u.

### 3. Checking perpendicularity to v

Similarly,

```math
(u\times v)\cdot v
=(6,-3,1)\cdot(0,1,3).
```

Therefore,

```math
(u\times v)\cdot v
=6(0)+(-3)(1)+1(3)
=-3+3
=0.
```

Thus, u × v is also perpendicular to v.

### 4. Computing v × u

Reversing the order gives

```math
v\times u=
(1(0)-3(2),\;
3(1)-0(0),\;
0(2)-1(1)).
```

Hence,

```math
\boxed{v\times u=(-6,3,-1)}.
```

### 5. Comparing the results

We observe that

```math
v\times u=-(u\times v).
```

The two cross products have the same length:

```math
\|u\times v\|
=\|v\times u\|
=\sqrt{6^2+(-3)^2+1^2}
=\sqrt{46}.
```

Both are perpendicular to the plane containing u and v, but they point in opposite directions.

Therefore, the cross product is anti-commutative: reversing the order reverses its orientation. The orientation is determined by the right-hand rule.
