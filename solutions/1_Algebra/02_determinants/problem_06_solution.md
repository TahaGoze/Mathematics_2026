# Exercise 6 - Parameter and Invertibility

## Question

Given

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

Find all values of $t$ for which $A(t)$ is not invertible. Explain the connection with its determinant.

## Solution

For a 2x2 matrix, I use $ad-bc$.

$$
\det A(t)=t\cdot t-1\cdot 2=t^2-2
$$

A matrix is not invertible when its determinant is zero.

$$
t^2-2=0
$$

$$
t^2=2 \quad \Rightarrow \quad t=\sqrt{2}\text{ or }t=-\sqrt{2}
$$

So the matrix is not invertible for $t=\pm\sqrt{2}$.

## Verification

For either value, $t^2=2$.

The first row is $(t,1)$. Multiplying it by $t$ gives $(t^2,t)=(2,t)$, which is the second row.

The rows are dependent, so the determinant is zero.
