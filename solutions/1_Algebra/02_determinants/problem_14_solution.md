# Exercise 14 - A System of Equations and the Determinant

## Question

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}
$$

Find all values of $k$ for which the system has exactly one solution for every $b$.

For the remaining value, give one example of $b$ with infinitely many solutions and one example with no solution.

## Solution

### 1. Exactly one solution

First, I calculate the determinant:

$$
\det A=1\cdot4-2\cdot k=4-2k
$$

A square matrix has exactly one solution for every $b$ when its determinant is not zero.

$$
4-2k\neq0
$$

So the condition is $k\neq2$.

### 2. When k = 2

For $k=2$, the matrix becomes

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix}
$$

The second row is twice the first row. The system is

$$
x_1+2x_2=b_1
$$

$$
2x_1+4x_2=b_2
$$

**Example with infinitely many solutions**

Choose

$$
b=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

Both equations reduce to $x_1+2x_2=1$.

We can choose any $x_2$ and take $x_1=1-2x_2$. Therefore, there are infinitely many solutions.

**Example with no solution**

Choose

$$
b=
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}
$$

The first equation says $x_1+2x_2=1$. Multiplying it by 2 gives $2x_1+4x_2=2$.

But the second equation requires $2x_1+4x_2=0$. Both cannot be true, so there is no solution.

## Verification

For $k=2$:

$$
\det A=4-2\cdot2=0
$$

This agrees with the dependent rows.

For $k\neq2$, the determinant is nonzero, so $A$ is invertible and $Ax=b$ has exactly one solution for every $b$.
