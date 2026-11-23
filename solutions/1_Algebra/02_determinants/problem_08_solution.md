# Exercise 8 - Determinant of a Product

## Question

Let $A$ and $B$ be square matrices with $\det A=3$ and $\det B=-5$.

Find $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two are equal even though $AB$ and $BA$ are usually different.

## Solution

The property I use is:

$$
\det(AB)=\det A\cdot\det B
$$

First:

$$
\det(AB)=3\cdot(-5)=-15
$$

For the reverse order:

$$
\det(BA)=(-5)\cdot3=-15
$$

Since $\det A=3\neq0$, the inverse $A^{-1}$ exists.

$$
\det(A^{-1})=\frac{1}{\det A}=\frac13
$$

Therefore:

$$
\det(A^{-1}B)=\frac13\cdot(-5)=-\frac53
$$

## Verification and Explanation

Both $\det(AB)$ and $\det(BA)$ are $-15$ because ordinary number multiplication is commutative:

$$
3(-5)=(-5)3
$$

The matrices $AB$ and $BA$ may still be different. Only their determinants must be equal.
