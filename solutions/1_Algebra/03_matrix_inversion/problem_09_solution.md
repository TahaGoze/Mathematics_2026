# Exercise 9 - Matrix Equation

## Question

Given the matrices

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
$$

solve the matrix equation $AX=B$ for $X$. Before calculating, decide on which side of the equation to multiply by $A^{-1}$. Check the result by calculating $AX$.

## Solution

Since $A$ is on the left side of $X$ in $AX=B$, I must multiply both sides by $A^{-1}$ from the left:

$$
A^{-1}AX=A^{-1}B
$$

Because $A^{-1}A=I$, this becomes

$$
X=A^{-1}B
$$

First, I find the inverse of $A$. Its determinant is

$$
\det A=1\cdot1-2\cdot0=1
$$

Using the inverse formula for a 2x2 matrix gives

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
$$

Now I calculate $X$ by multiplying $A^{-1}$ and $B$:

$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
$$

Each entry is found by multiplying a row by a column:

$$
X=
\begin{pmatrix}
1\cdot3+(-2)\cdot2 & 1\cdot1+(-2)\cdot4 \\
0\cdot3+1\cdot2 & 0\cdot1+1\cdot4 \\
\end{pmatrix}
$$

So the answer is

$$
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

Multiplying by $A^{-1}$ on the right would not cancel $A$, because the order of matrix multiplication matters.

## Verification

I substitute $X$ into the original equation:

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

Calculating the entries gives

$$
AX=
\begin{pmatrix}
1\cdot(-1)+2\cdot2 & 1\cdot(-7)+2\cdot4 \\
0\cdot(-1)+1\cdot2 & 0\cdot(-7)+1\cdot4 \\
\end{pmatrix}
$$

Therefore,

$$
AX=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=B
$$

The product equals the given matrix $B$, so the solution is correct.
