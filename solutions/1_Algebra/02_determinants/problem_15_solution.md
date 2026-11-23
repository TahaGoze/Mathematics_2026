# Exercise 15 - Combining Determinant Properties

## Question

Let $A$ and $B$ be invertible 2x2 matrices with

$$
\det A=-2,\qquad \det B=3
$$

Without finding the entries of the matrices, calculate

$$
\det(B^{-1}A^TB)
$$

State the determinant properties used in order and explain why the factors involving $B$ cancel.

## Solution

First, I use the determinant property for a product:

$$
\det(B^{-1}A^TB)=\det(B^{-1})\cdot\det(A^T)\cdot\det B
$$

Since $B$ is invertible, I can use the inverse property:

$$
\det(B^{-1})=\frac{1}{\det B}=\frac{1}{3}
$$

Transposing a matrix does not change its determinant:

$$
\det(A^T)=\det A=-2
$$

Now I substitute the values:

$$
\det(B^{-1}A^TB)=\frac{1}{3}\cdot(-2)\cdot3=-2
$$

The factors involving $B$ cancel because

$$
\det(B^{-1})\cdot\det B=\frac13\cdot3=1
$$

## Verification

I can also group the determinant factors in a different order:

$$
\det(B^{-1}A^TB)=\det(A^T)\cdot\big(\det(B^{-1})\cdot\det B\big)
$$

$$
\det(B^{-1}A^TB)=(-2)\cdot1=-2
$$

Both ways give the same result, so the determinant is $-2$.
