# Exercise 14 - A Small Change in the Right-Hand Side

## Question

Compare the following two systems.

**System 1:**

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3. \\
\end{cases}
$$

**System 2:**

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1. \\
\end{cases}
$$

Check whether each system is consistent, and explain why a small change in the last right-hand side can change the type of the system.

## Solution

### System 1

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3 \\
\end{pmatrix}
$$

I first eliminate the entries under the first pivot using two row operations:

$$
R_2\leftarrow R_2-2R_1
$$

$$
R_3\leftarrow R_3-3R_1
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}
$$

Now I subtract row 2 from row 3:

$$
R_3\leftarrow R_3-R_2
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The last row represents $0=0$, which is always true. The second row gives

$$
-3y=-3,\qquad y=1
$$

From the first row,

$$
x+y=2,\qquad x=1
$$

Therefore, System 1 is consistent and has exactly one solution:

$$
(x,y)=(1,1)
$$

### System 2

Only the last right-hand side changes from $3$ to $3.1$. Its augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3.1 \\
\end{pmatrix}
$$

I repeat the same elimination steps:

$$
R_2\leftarrow R_2-2R_1
$$

$$
R_3\leftarrow R_3-3R_1
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -2.9 \\
\end{pmatrix}
$$

Next, I subtract row 2 from row 3:

$$
R_3\leftarrow R_3-R_2
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0.1 \\
\end{pmatrix}
$$

The last row represents $0=0.1$. This is impossible, so System 2 is inconsistent and has no solution.

### Why the small change matters

The sum of the first two equations is

$$
(x+y)+(2x-y)=2+1
$$

After simplifying, this gives

$$
3x=3
$$

Thus, in System 1 the third equation already follows from the first two and adds no new information. In System 2, the third equation asks for $3x=3.1$ instead. This contradicts the value $3x=3$ that is forced by the first two equations.

Even a change of $0.1$ can make the equations incompatible because an exact equality must hold. The first system has one solution, while the second has none.

## Verification

For System 1, substitute $x=1$ and $y=1$ into all three original equations:

$$
1+1=2
$$

$$
2\cdot1-1=1
$$

$$
3\cdot1=3
$$

All three equations are satisfied.

For System 2, the first two equations still require $x=1$ and $y=1$. However, substituting $x=1$ into its third equation would require

$$
3\cdot1=3.1
$$

This is false. It confirms the contradiction found in the last row of the augmented matrix.
