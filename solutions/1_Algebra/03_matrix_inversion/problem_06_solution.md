# Exercise 6 - Solving a System Using the Inverse

## Question

Solve $Ax=b$, where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

and

$$
b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$

Use $x=A^{-1}b$. Then substitute the result back into $Ax=b$ to verify the solution.

## Solution

First, I calculate the determinant of $A$:

$$
\det A=2\cdot3-1\cdot1=5
$$

Since the determinant is not zero, the inverse exists.

Using the formula for a 2x2 matrix, I get

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

To solve the system, I multiply the inverse by $b$:

$$
x=A^{-1}b=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$

The first entry is $3\cdot5-1\cdot7=8$, and the second entry is $-1\cdot5+2\cdot7=9$.

Thus,

$$
x=
\frac{1}{5}
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}
$$

The solution is

$$
x=
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}
$$

## Verification

I substitute the result into the original equation:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}
$$

The first entry is

$$
2\cdot\frac85+\frac95=\frac{16+9}{5}=5
$$

The second entry is

$$
\frac85+3\cdot\frac95=\frac{8+27}{5}=7
$$

Therefore,

$$
Ax=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$

This is the given vector $b$, so the solution is correct.
