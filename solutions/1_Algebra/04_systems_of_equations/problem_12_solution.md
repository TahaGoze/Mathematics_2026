# Exercise 12 - Homogeneous System

## Question

Solve the homogeneous system

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0. \\
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

I start with the augmented matrix:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

First, I subtract twice the first row from the second row:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

Next, I subtract the first row from the third row:

$$
R_3\leftarrow R_3-R_1
$$

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

I swap rows 2 and 3 to get row echelon form:

$$
R_2\leftrightarrow R_3
$$

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row gives

$$
-3y+3z=0
$$

Therefore, $y=z$.

There are three unknowns and two pivots, in the columns for $x$ and $y$. The third column has no pivot, so I choose $z$ as the free variable.

Let $z=s$, where $s$ is any real number. Then $y=s$.

Substituting into the first row:

$$
x+2s-s=0
$$

Thus, $x=-s$.

The complete parametric solution is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
-s \\
s \\
s \\
\end{pmatrix},
\qquad s\in\mathbb{R}
$$

There are infinitely many solutions because $s$ can be any real number.

## Verification

I substitute $x=-s$, $y=s$, and $z=s$ into each original equation.

First equation:

$$
-s+2s-s=0
$$

Second equation:

$$
2(-s)+4s-2s=0
$$

Third equation:

$$
-s-s+2s=0
$$

All three equations are satisfied for every real $s$.

In particular, setting $s=0$ gives $(x,y,z)=(0,0,0)$. In any homogeneous system, every equation has zero on the right-hand side. Setting every unknown to zero makes every left-hand side zero as well. Therefore, the zero vector always solves any homogeneous linear system.
