# Exercise 10 - Inverse of a Diagonal Matrix

## Question

Given the diagonal matrices

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

and

$$
E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

Decide which matrix is invertible without using Gauss-Jordan elimination. Find the inverse of the invertible matrix and check it by multiplication.

## Solution

For a diagonal matrix, the determinant is the product of the diagonal entries.

First, I calculate the determinant of $D$:

$$
\det D=2\cdot(-3)\cdot5=-30
$$

Since the determinant is not zero, $D$ is invertible.

For the matrix $E$, the determinant is

$$
\det E=2\cdot0\cdot5=0
$$

So $E$ is not invertible. It also has a zero second row, which confirms this result.

To find the inverse of a diagonal matrix, I take the reciprocal of each nonzero diagonal entry. The off-diagonal entries stay zero.

Therefore,

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}
$$

## Verification

I check the result by multiplying $D$ by its inverse:

$$
DD^{-1}=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}
$$

The diagonal entries of the product are $2\cdot\frac12=1$, $(-3)\cdot(-\frac13)=1$, and $5\cdot\frac15=1$. All off-diagonal entries are zero.

Thus,

$$
DD^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
=I
$$

The product is the identity matrix, so the inverse of $D$ is correct. No Gauss-Jordan elimination was needed.
