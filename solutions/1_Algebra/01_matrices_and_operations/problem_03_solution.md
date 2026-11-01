# Problem 3 Solution

### Rule of Matrix Multiplication Compatibility
Two matrices $A$ (size $m \times n$) and $B$ (size $p \times q$) can be multiplied in the order $AB$ if and only if the inner dimensions match ($n = p$). The resulting matrix will have the dimensions $m \times q$.

### Analysis of Products

1. **$AB$ ($2 \times 3$ and $3 \times 4$)**
   - Inner dimensions match ($3 = 3$).
   - **Defined**, resulting size: $2 \times 4$

2. **$BA$ ($3 \times 4$ and $2 \times 3$)**
   - Inner dimensions do not match ($4 \neq 2$).
   - **Undefined**

3. **$BC$ ($3 \times 4$ and $4 \times 2$)**
   - Inner dimensions match ($4 = 4$).
   - **Defined**, resulting size: $3 \times 2$

4. **$CB$ ($4 \times 2$ and $3 \times 4$)**
   - Inner dimensions do not match ($2 \neq 3$).
   - **Undefined**

5. **$AC$ ($2 \times 3$ and $4 \times 2$)**
   - Inner dimensions do not match ($3 \neq 4$).
   - **Undefined**

6. **$CA$ ($4 \times 2$ and $2 \times 3$)**
   - Inner dimensions match ($2 = 2$).
   - **Defined**, resulting size: $4 \times 3$

7. **$AD$ ($2 \times 3$ and $2 \times 2$)**
   - Inner dimensions do not match ($3 \neq 2$).
   - **Undefined**

8. **$DA$ ($2 \times 2$ and $2 \times 3$)**
   - Inner dimensions match ($2 = 2$).
   - **Defined**, resulting size: $2 \times 3$
