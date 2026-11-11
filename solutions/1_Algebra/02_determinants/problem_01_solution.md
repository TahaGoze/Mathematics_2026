# Exercise 1 - Determinant of a 2x2 Matrix

## Question

Calculate the determinants of:

$$
A = \begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}
$$

Find which matrix is invertible and justify the answer using the determinants.

## Solution

For a 2x2 matrix, the determinant formula is:

$\det = ad-bc$

First matrix:

$\det(A) = 3 \cdot  4 - (-2 \cdot  5)$

= 12 + 10

$\det(A) = 22$

Second matrix:

$\det(B) = 1 \cdot  14 - 7 \cdot  2$

= 14 - 14

$\det(B) = 0$

The first matrix is invertible because its determinant is not zero.

The second matrix is not invertible because its determinant is zero.

## Verification

The first row of $B$ is $(1,7)$, and the second row is $(2,14)$.

Since $(2,14)=2(1,7)$, the second row is twice the first one. The rows are dependent, so the determinant of $B$ is zero.
