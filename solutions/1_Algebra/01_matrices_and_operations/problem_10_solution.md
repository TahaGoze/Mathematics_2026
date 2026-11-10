# Exercise 10 - Columns of a Matrix Product

## Question

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

Find Ab1, Ab2 and AB. Explain the connection.

## Solution

The columns of B are:

$$
b_{1} = \begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}
$$

$$
b_{2} = \begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
$$

First, calculate Ab1:

First row: $1(1) + 2(-1) + 0(3) = -1$

Second row: $0(1) + 1(-1) + 1(3) = 2$

$$
Ab1 = \begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

Now calculate Ab2:

First row: $1(2) + 2(0) + 0(1) = 2$

Second row: $0(2) + 1(0) + 1(1) = 1$

$$
Ab2 = \begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

Now multiply A by B:

$$
AB = \begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

## Verification and Explanation

The first column of $AB$ is $Ab_1$:

$$
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

The second column of $AB$ is $Ab_2$:

$$
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

This happens because multiplying A by B means multiplying A by each column of B.
