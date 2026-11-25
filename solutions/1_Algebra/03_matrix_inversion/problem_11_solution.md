# Exercise 11 - Parameter and Invertibility

## Question

For the matrix

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is invertible. Then give a formula for $A(t)^{-1}$ and explain what happens to the formula for the excluded values of $t$.

## Solution

First, I calculate the determinant using $ad-bc$:

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2
$$

A square matrix is invertible when its determinant is not zero.

$$
1-t^2\neq0
$$

The determinant equals zero when $t=1$ or $t=-1$.

Therefore, the matrix is invertible for all values except $t=1$ and $t=-1$.

For an invertible 2x2 matrix, I use the inverse formula. Since the determinant is $1-t^2$, I get

$$
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}
$$

This formula is valid only when $t\neq1$ and $t\neq-1$.

For $t=1$ and $t=-1$, the denominator becomes zero, so the formula is undefined. The rows are also dependent at these values. Therefore, no inverse exists.

## Verification

To check the formula, I multiply $A(t)$ by the proposed inverse:

$$
A(t)A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}
$$

Multiplying the rows and columns gives

$$
A(t)A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & 0 \\
0 & 1-t^2 \\
\end{pmatrix}
$$

For $t\neq1$ and $t\neq-1$, I can cancel $1-t^2$:

$$
A(t)A(t)^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

This confirms the inverse formula and its restriction on $t$.
