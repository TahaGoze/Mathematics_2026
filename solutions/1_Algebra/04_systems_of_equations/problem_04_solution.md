# Exercise 4 - Infinitely Many Solutions

## Question

Solve the system

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0. \\
\end{cases}
$$

Write all solutions in parametric form, identify a free variable, and choose one parameter value to verify that the corresponding point satisfies the original system.

## Solution

First, I write the augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

I eliminate the first entry in row 2:

$$
R_2 \leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

Next, I subtract row 1 from row 3:

$$
R_3 \leftarrow R_3-R_1
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

To write the matrix in row echelon form, I swap rows 2 and 3:

$$
R_2 \leftrightarrow R_3
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row gives

$$
-2y=-2
$$

Thus, $y=1$.

The first row is $x+y+z=2$. Substituting $y=1$ gives

$$
x+z=1
$$

There are three unknowns but only two nonzero equations after elimination. I can choose $z$ freely.

Let $z=t$, where $t$ is any real number. Then

$$
x=1-t,\qquad y=1,\qquad z=t
$$

Therefore, the parametric solution is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
1-t \\
1 \\
t \\
\end{pmatrix},
\qquad t\in\mathbb{R}
$$

Because $t$ can take any real value, the system has infinitely many solutions.

## Verification

I choose $t=0$. Then $x=1$, $y=1$, and $z=0$.

Substituting into the first equation:

$$
1+1+0=2
$$

Substituting into the second equation:

$$
2\cdot1+2\cdot1+2\cdot0=4
$$

Substituting into the third equation:

$$
1-1+0=0
$$

All three original equations are satisfied. The row operations also show that the second equation is redundant and that the free variable $z=t$ produces infinitely many solutions.
