# Exercise 1 - From a System to a Matrix

## Question

Write the following system in the form $Ax=b$:

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

Identify the coefficient matrix $A$, the vector of unknowns $x$, and the right-hand side vector $b$. Explain how each row of $A$ corresponds to one equation.

## Solution

The coefficient matrix contains the numbers multiplying $x$, $y$, and $z$ in each equation, in that order.

From the first equation, $2x-y+z=4$, I take the coefficients $(2,-1,1)$.

From the second equation, $x+3y-2z=1$, I take the coefficients $(1,3,-2)$.

From the third equation, $3x+y+z=7$, I take the coefficients $(3,1,1)$.

Therefore, the coefficient matrix is

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
$$

The vector of unknowns is

$$
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
$$

The right-hand side vector contains the numbers after the equals signs in the three equations:

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

The system in matrix form is

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

Thus, $Ax=b$ represents all three original equations at once.

## Verification

To check the matrix form, I multiply each row of $A$ by the column vector of unknowns:

$$
Ax=
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}
$$

These entries are exactly the left-hand sides of the original equations, in the same order. According to the given system, they equal $4$, $1$, and $7$.

Therefore,

$$
Ax=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
=b
$$

The matrix equation matches the original system.
