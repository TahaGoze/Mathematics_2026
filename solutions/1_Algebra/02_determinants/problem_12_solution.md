# Exercise 12 - A Parameter Revealed by a Row Operation

## Question

Given the matrix

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Find all values of $t$ for which $A(t)$ is not invertible.

Before calculating the determinant, use $R_2\leftarrow R_2-2R_1$. Explain what happens to the rows for the value of $t$ found.

## Solution

First, subtract twice the first row from the second row:

$$
R_2\leftarrow R_2-2R_1
$$

$$
(2,4,t)-2(1,2,3)=(0,0,t-6)
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Adding a multiple of one row to another does not change the determinant.

I expand along the first column because it has two zeros:

$$
\det A(t)=1\big(0\cdot1-(t-6)\cdot1\big)=6-t
$$

A square matrix is not invertible when its determinant is zero.

$$
6-t=0
$$

Therefore, $t=6$.

## Verification

For $t=6$, the original second row becomes $(2,4,6)$, which is twice the first row $(1,2,3)$.

The rows are dependent, so the determinant is zero. This confirms that the matrix is not invertible for $t=6$.
