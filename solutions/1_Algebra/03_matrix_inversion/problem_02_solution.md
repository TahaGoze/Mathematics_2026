# Exercise 2 - Formula for a 2x2 Matrix

## Question

Find the inverse of the matrix

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

Use the formula for a $2\times2$ matrix. Check the answer by multiplying the inverse by $A$.

## Solution

For a $2\times2$ matrix, the inverse formula is

$$
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}^{-1} = \frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}
$$

First, I calculate the determinant of $A$:

$$
\det A=3\cdot4-2\cdot5=12-10=2
$$

Because the determinant is not zero, the inverse exists.

I substitute the entries into the formula:

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
$$

Multiplying by $\frac12$ gives

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac52 & \frac32 \\
\end{pmatrix}
$$

## Verification

To check the answer, I calculate $AA^{-1}$ using row-by-column multiplication:

$$
AA^{-1}=
\begin{pmatrix}
3\cdot2+2\cdot(-\frac52) & 3\cdot(-1)+2\cdot\frac32 \\
5\cdot2+4\cdot(-\frac52) & 5\cdot(-1)+4\cdot\frac32 \\
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

The product is the identity matrix, so the inverse is correct.
