# Exercise 7 - Inverse of a Product

## Question

Given the matrices

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

Calculate $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that both results are equal and explain why the order of the matrices is reversed.

## Solution

### 1. Finding the inverse of AB

First, multiply $A$ and $B$:

$$
AB=
\begin{pmatrix}
1\cdot2+1\cdot0 & 1\cdot0+1\cdot3 \\
0\cdot2+1\cdot0 & 0\cdot0+1\cdot3 \\
\end{pmatrix}
$$

This gives

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
$$

The determinant is

$$
\det(AB)=2\cdot3-3\cdot0=6
$$

Since the determinant is not zero, the inverse exists. Using the inverse formula for a 2x2 matrix:

$$
(AB)^{-1}=
\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
$$

After multiplying by $\frac16$, I get

$$
(AB)^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
$$

### 2. Finding the product of the inverses

For $A$, the determinant is $1$, so its inverse is

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

The inverse of the diagonal matrix $B$ is

$$
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}
$$

Multiplying in the order $B^{-1}A^{-1}$ gives

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

The product is

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
$$

Both calculations give the same matrix.

### 3. Explaining the reversed order

In the product $AB$, the transformation $B$ acts first and then $A$ acts. To undo the product, we undo $A$ first with $A^{-1}$ and then undo $B$ with $B^{-1}$.

Therefore, the inverse of a product has the reversed order:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

## Verification

I check the answer by multiplying $AB$ by the inverse:

$$
(AB)(AB)^{-1}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
$$

The four entries are

$$
\begin{pmatrix}
2\cdot\frac12+3\cdot0 & 2\cdot(-\frac12)+3\cdot\frac13 \\
0\cdot\frac12+3\cdot0 & 0\cdot(-\frac12)+3\cdot\frac13 \\
\end{pmatrix}
$$

They simplify to the identity matrix:

$$
(AB)(AB)^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

This confirms the result.
