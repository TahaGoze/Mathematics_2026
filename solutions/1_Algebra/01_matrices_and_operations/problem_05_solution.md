# Exercise 5 - Matrix Times Vector

## Question

Given:

$$
A = \begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
$$

$$
x = \begin{pmatrix}
4 \\
2 \\
\end{pmatrix}
$$

1. Calculate Ax.
2. Express Ax as a linear combination of the columns of A.

## Solution

### 1. Calculate Ax

I multiplied each row of A by vector x.

- First row: 2 x 4 + (-1) x 2 = 6
- Second row: 1 x 4 + 3 x 2 = 10

**Result:**

$$
Ax = \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

### 2. Linear Combination

The columns of A are:

First column:

$$
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

Second column:

$$
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

Using the numbers 4 and 2 from vector x:

$$
4 x \begin{pmatrix}
2 \\
1 \\
\end{pmatrix} + 2 x \begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

$$
= \begin{pmatrix}
8 \\
4 \\
\end{pmatrix} + \begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
$$

$$
= \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

### Verification

Both methods give the same result:

$$
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

So the calculation is correct.
