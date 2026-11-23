# Exercise 4 - Gauss-Jordan

## Question

Find the inverse of

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}
$$

using the Gauss-Jordan method. Show the augmented matrix $[A\mid I]$ after each row operation. Explain why getting the identity matrix on the left gives the inverse on the right.

## Solution

I start with the matrix $A$ and the identity matrix $I$ side by side:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

**Step 1.** Subtract three times the first row from the second row:

$$
R_2 \leftarrow R_2-3R_1
$$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

**Step 2.** Multiply the second row by $-1$ so that its leading entry is $1$:

$$
R_2 \leftarrow -R_2
$$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

**Step 3.** Subtract twice the second row from the first row:

$$
R_1 \leftarrow R_1-2R_2
$$

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

The left side is now the identity matrix. Therefore, the matrix on the right is

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
$$

The same row operations were applied to $A$ and to $I$. If these operations together are represented by a matrix $E$, then $EA=I$ and $EI=E$. This is why the right side becomes $A^{-1}$ when the left side becomes $I$.

## Verification

I check the answer by multiplying $A$ by the result:

$$
AA^{-1}=
\begin{pmatrix}
1\cdot(-5)+2\cdot3 & 1\cdot2+2\cdot(-1) \\
3\cdot(-5)+5\cdot3 & 3\cdot2+5\cdot(-1) \\
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

The product is the identity matrix, so the inverse is correct.
