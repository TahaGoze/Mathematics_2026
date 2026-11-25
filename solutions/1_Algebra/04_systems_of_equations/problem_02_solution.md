# Exercise 2 - Gaussian Elimination - One Solution

## Question

Solve the following system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2. \\
\end{cases}
$$

After finding the solution, substitute it into all three original equations and check that they are consistent.

## Solution

I start by writing the augmented matrix of the system:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

**Step 1.** Subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

**Step 2.** Subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

**Step 3.** Swap the second and third rows to use the leading coefficient $1$:

$$
R_2 \leftrightarrow R_3
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

**Step 4.** Add three times the second row to the third row:

$$
R_3 \leftarrow R_3+3R_2
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

The matrix is now in row echelon form. I use back-substitution.

From the third row:

$$
-7z=-21
$$

$$
z=3
$$

From the second row, $y-2z=-4$:

$$
y-2\cdot3=-4
$$

$$
y=2
$$

From the first row, $x+y+z=6$:

$$
x+2+3=6
$$

$$
x=1
$$

Therefore, the solution is

$$
x=1,\qquad y=2,\qquad z=3
$$

In vector form:

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
1 \\
2 \\
3 \\
\end{pmatrix}
$$

## Verification

I substitute $x=1$, $y=2$, and $z=3$ into each original equation.

First equation:

$$
1+2+3=6
$$

Second equation:

$$
2\cdot1-2+3=3
$$

Third equation:

$$
1+2\cdot2-3=2
$$

All three equations are satisfied. Since Gaussian elimination gives a pivot for every unknown, the system has exactly one solution.
