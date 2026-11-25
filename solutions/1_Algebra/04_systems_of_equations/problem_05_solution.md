# Exercise 5 - Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how many variables can be chosen freely and why.

## Solution

The given matrix is already in row echelon form. It represents the equations

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0. \\
\end{cases}
$$

The first two rows contain pivots in the columns for $x$ and $y$. The third row is all zeros and does not add another restriction.

There are three unknowns but only two pivot columns. Therefore, there is one free variable: $z$.

I choose

$$
z=t,\qquad t\in\mathbb{R}
$$

From the second row:

$$
y+2z=1
$$

Substituting $z=t$ gives

$$
y=1-2t
$$

From the first row:

$$
x+2y-z=3
$$

Substituting $y=1-2t$ and $z=t$:

$$
x+2(1-2t)-t=3
$$

Simplifying:

$$
x+2-5t=3
$$

Therefore,

$$
x=1+5t
$$

The solution in parametric form is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
1+5t \\
1-2t \\
t \\
\end{pmatrix},
\qquad t\in\mathbb{R}
$$

Because $t$ can be any real number, the system has infinitely many solutions.

## Verification

Substitute the parametric solution into the first equation:

$$
(1+5t)+2(1-2t)-t=3
$$

The left-hand side simplifies to $3$, so the first equation is satisfied for every $t$.

For the second equation:

$$
(1-2t)+2t=1
$$

The second equation is also satisfied for every $t$.

The third row is $0=0$, which is always true.

As an additional check, choose $t=1$. Then

$$
x=6,\qquad y=-1,\qquad z=1
$$

Substituting these values gives

$$
6+2(-1)-1=3
$$

and

$$
-1+2(1)=1
$$

Thus all three rows are satisfied. One free variable remains, so the system has infinitely many solutions.
