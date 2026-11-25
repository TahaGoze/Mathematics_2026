# Exercise 14 - A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix $A$ satisfies

$$
A^2=I
$$

Show that $A^{-1}=A$. Then give an example of a $2\times2$ matrix different from both $I$ and $-I$ that satisfies this condition. Verify the example by matrix multiplication.

## Solution

By definition, the inverse of a square matrix $A$ is a matrix that gives the identity matrix when multiplied by $A$ on either side.

The given condition is

$$
A^2=AA=I
$$

This means that multiplying $A$ by itself gives the identity matrix. So $A$ is its own inverse:

$$
A^{-1}=A
$$

For a specific example, I choose

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

This matrix is different from $I$ because the entries on its diagonal are zero, and it is also different from $-I$ because it has nonzero off-diagonal entries.

## Verification

I multiply the example matrix by itself:

$$
A^2=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

Calculating each entry by row-column multiplication gives

$$
A^2=
\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \\
\end{pmatrix}
$$

Therefore,

$$
A^2=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

The matrix satisfies $A^2=I$ and is not $I$ or $-I$. The multiplication confirms that its inverse is the same matrix.
