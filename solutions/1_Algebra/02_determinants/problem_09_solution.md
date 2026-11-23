# Exercise 9 - Area and the Determinant

## Question

The vectors are

$$
u=\begin{pmatrix}
3 \\
1 \\
\end{pmatrix}
$$

$$
v=\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

Find the area of the parallelogram using a determinant. Reverse the order of the vectors, and explain what changes in the determinant and the area.

## Solution

I use $u$ and $v$ as the columns of a matrix.

$$
A=\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
$$

Its determinant is:

$$
\det A=3\cdot4-1\cdot1=12-1=11
$$

The area is the absolute value:

$$
\mathrm{Area}=|11|=11
$$

Now reverse the vectors:

$$
B=\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
$$

$$
\det B=1\cdot1-3\cdot4=1-12=-11
$$

## Verification and Explanation

Swapping two columns changes the sign of the determinant, so $11$ becomes $-11$.

The area does not change because $|-11|=11$.

Final area: $11$ square units.
