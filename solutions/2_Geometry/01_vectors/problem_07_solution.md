# Exercise 7. Linear Dependence Without Heavy Computation

## Question

Given

```math
u=(1,2,3),
\qquad
v=(2,4,6),
\qquad
w=(0,1,1),
```

identify a specific relation between u and v, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

## Solution

### 1. Identifying the relation

Each component of v is twice the corresponding component of u:

```math
v=(2,4,6)=2(1,2,3)=2u.
```

Therefore,

```math
\boxed{v=2u}.
```

The vectors u and v are parallel and have the same orientation.

### 2. Testing linear independence

Vectors are linearly independent if the only combination giving the zero vector has all coefficients equal to zero.

Here, the relation v=2u gives

```math
2u-v+0w=(0,0,0).
```

Indeed,

```math
2(1,2,3)-(2,4,6)+0(0,1,1)
=(0,0,0).
```

The coefficients 2, -1, and 0 are not all zero. Thus, we have a nontrivial linear relation, proving that

```math
\boxed{u,v,w\text{ are linearly dependent}}.
```

A coefficient in a dependence relation is allowed to be zero; only one coefficient needs to be nonzero.

### 3. Why no long calculation is needed

The dependence is already visible in the relation between u and v. Adding the third vector w cannot remove that existing relation.

Therefore, there is no need to compute a determinant or perform elimination. The simple observation v=2u is enough to prove that the three vectors are linearly dependent.
