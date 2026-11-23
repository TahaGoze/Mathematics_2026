# Exercise 1 - Definition of the Inverse

## Question

Given the matrices

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

Check without using the inverse formula whether $B=A^{-1}$. Calculate $AB$ and $BA$, and explain the result using the definition of the inverse.

## Solution

Two square matrices are inverses of each other if both products give the identity matrix.

First, I calculate $AB$ by multiplying rows of $A$ by columns of $B$:

$$
AB=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

Next, I calculate $BA$ in the opposite order:

$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

## Verification

Both $AB$ and $BA$ are equal to the identity matrix $I$.

By the definition of the inverse, $B=A^{-1}$. I checked this using matrix multiplication, without an inverse formula.
