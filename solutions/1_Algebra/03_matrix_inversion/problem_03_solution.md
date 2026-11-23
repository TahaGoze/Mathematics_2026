# Exercise 3 - When Does the Inverse Not Exist?

## Question

For the matrix

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

Explain in two ways why $A^{-1}$ does not exist: by calculating the determinant and by showing dependence between the rows.

## Solution

### 1. Using the determinant

For a 2x2 matrix, the determinant is $ad-bc$.

$$
\det A=2\cdot2-4\cdot1=4-4=0
$$

A square matrix has an inverse only if its determinant is not zero.

Since $\det A=0$, the inverse $A^{-1}$ does not exist.

### 2. Using dependence between the rows

The first row is $(2,4)$ and the second row is $(1,2)$.

The first row is twice the second row:

$$
R_1=2R_2
$$

This means the rows are linearly dependent. A matrix with dependent rows is not invertible.

## Verification

Subtracting twice the second row from the first gives

$$
R_1\leftarrow R_1-2R_2
$$

The resulting matrix is

$$
\begin{pmatrix}
0 & 0 \\
1 & 2 \\
\end{pmatrix}
$$

It has a zero row, so its determinant is zero. This agrees with the first method and confirms that $A^{-1}$ does not exist.
