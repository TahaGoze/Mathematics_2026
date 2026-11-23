# Exercise 11 - Shortening the Calculation with Row Operations

## Question

Calculate the determinant of

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

Use row operations to create as many zeros as possible. State which operations do not change the determinant.

## Solution

First, I subtract the first row from the second row:

$$
R_2 \leftarrow R_2-R_1
$$

This gives

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

Next, I subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

Now the matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

Finally, I subtract twice the second row from the third row:

$$
R_3 \leftarrow R_3-2R_2
$$

The result is an upper triangular matrix:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

Every operation subtracted a multiple of one row from another row. Such operations do not change the determinant.

For a triangular matrix, the determinant is the product of the diagonal entries.

$$
\det A=1\cdot1\cdot1=1
$$

## Verification

I also check by expanding the original matrix along its first row:

$$
\det A=1(3\cdot6-4\cdot4)-2(1\cdot6-4\cdot1)+3(1\cdot4-3\cdot1)
$$

$$
\det A=2-4+3=1
$$

Both methods give the same determinant.
