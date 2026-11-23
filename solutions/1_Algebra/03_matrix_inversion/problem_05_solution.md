# Exercise 5 - A 3x3 Matrix

## Question

Use Gauss-Jordan elimination to find the inverse of

$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}
$$

Show the row operations and check the answer by matrix multiplication.

## Solution

I start by placing the identity matrix next to $A$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1 \\
\end{pmatrix}
$$

**Step 1.** Subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}
$$

**Step 2.** Add the second row to the third row to make another zero:

$$
R_3 \leftarrow R_3+R_2
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1 \\
\end{pmatrix}
$$

**Step 3.** Divide the third row by $2$:

$$
R_3 \leftarrow \frac12 R_3
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

**Step 4.** Subtract the third row from the second row:

$$
R_2 \leftarrow R_2-R_3
$$

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

**Step 5.** Subtract the second row from the first row:

$$
R_1 \leftarrow R_1-R_2
$$

$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac12 & -\frac12 & \frac12 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

The left side has become the identity matrix. Because the same row operations were applied to both sides, the right side is the inverse of $A$.

Therefore,

$$
A^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 & \frac12 \\
\frac12 & \frac12 & -\frac12 \\
-\frac12 & \frac12 & \frac12 \\
\end{pmatrix}
$$

## Verification

I check the answer by multiplying $A$ by $A^{-1}$:

$$
AA^{-1}=
\frac12
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1 \\
\end{pmatrix}
$$

Multiplying each row by each column gives

$$
AA^{-1}=
\frac12
\begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2 \\
\end{pmatrix} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
=I
$$

This confirms that the inverse is correct.
