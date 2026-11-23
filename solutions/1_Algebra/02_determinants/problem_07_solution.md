# Exercise 7 - Using Determinant Properties

## Question

Let $A$ be a 3x3 matrix with $\det A=-4$.

Find $\det(2A)$, $\det(A^T)$, $\det(A^2)$ and $\det(-A)$. Explain the properties used.

## Solution

### 1. det(2A)

For a 3x3 matrix, multiplying all entries by 2 multiplies the determinant by $2^3$.

$$
\det(2A)=2^3\det A=8(-4)=-32
$$

### 2. det(A^T)

Transposing a matrix does not change its determinant.

$$
\det(A^T)=\det A=-4
$$

### 3. det(A^2)

The determinant of a product is the product of the determinants.

$$
\det(A^2)=\det(A)\det(A)=(-4)^2=16
$$

### 4. det(-A)

Multiplying every entry by $-1$ multiplies the determinant by $(-1)^3$.

$$
\det(-A)=(-1)^3(-4)=4
$$

## Verification

The results use the scaling, transpose and product properties. I did not need the entries of $A$.

Final answers: $-32$, $-4$, $16$ and $4$.
