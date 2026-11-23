# Exercise 13 - Determinant by Elimination

## Question

Calculate the determinant of

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

Use elimination and state how every row operation affects the determinant.

## Solution

First, subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2-2R_1
$$

The second row becomes $(0,1,1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

This operation does not change the determinant because I subtracted a multiple of another row.

Next, subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

The third row becomes $(0,-2,-1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

This operation also does not change the determinant.

Finally, add twice the second row to the third row:

$$
R_3 \leftarrow R_3+2R_2
$$

The third row becomes $(0,0,1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

Again, adding a multiple of one row to another leaves the determinant unchanged.

The final matrix is upper triangular, so its determinant is the product of the diagonal entries:

$$
\det A=1\cdot1\cdot1=1
$$

## Verification

All three operations preserve the determinant. Since the final upper triangular matrix has determinant $1$, the original matrix also has determinant $1$.
