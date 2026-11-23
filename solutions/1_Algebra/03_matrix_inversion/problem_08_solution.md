# Exercise 8 - Inverse of a Transformation

## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of $S$ followed by $S^{-1}$ on a simple vector.

## Solution

The matrix $S$ multiplies the first coordinate by $2$ and the second coordinate by $\frac12$.

To undo this scaling, the inverse must multiply the first coordinate by $\frac12$ and the second coordinate by $2$.

So the inverse is

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}
$$

Geometrically, $S$ stretches the plane horizontally by a factor of $2$ and compresses it vertically by a factor of $\frac12$. The inverse does the opposite: it compresses horizontally by $\frac12$ and stretches vertically by $2$.

## Verification

I choose the vector

$$
v=
\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}
$$

First, I apply $S$:

$$
Sv=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}
$$

The result is

$$
Sv=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
$$

Then I apply $S^{-1}$ to the result:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
$$

This gives the original vector:

$$
S^{-1}(Sv)=
\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}
=v
$$

As another check, I multiply the matrices:

$$
S^{-1}S=
\begin{pmatrix}
\frac12\cdot2 & 0 \\
0 & 2\cdot\frac12 \\
\end{pmatrix}
$$

The product is the identity matrix:

$$
S^{-1}S=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

This confirms that $S^{-1}$ reverses the scaling done by $S$.
