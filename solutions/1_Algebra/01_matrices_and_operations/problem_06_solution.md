# Exercise 6 - Transpose

## Question

Given the matrices:

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

1. Calculate the transpose of A and B.
2. Calculate AB.
3. Verify that (AB)^T = B^T A^T.

## Solution

### 1. Transpose of A and B

To find the transpose, I change the rows into columns.

A is a 2x3 matrix, so A^T is 3x2.

$$
A^{T} = \begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

B is a 3x2 matrix, so B^T is 2x3.

$$
B^{T} = \begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

### 2. Calculate AB

I multiply each row of A by each column of B and add the results.

- Row 1, Column 1: 1x1 + 2x2 + 3x(-1) = 2
- Row 1, Column 2: 1x0 + 2x1 + 3x3 = 11
- Row 2, Column 1: 4x1 + 5x2 + 6x(-1) = 8
- Row 2, Column 2: 4x0 + 5x1 + 6x3 = 23

**Result:**

$$
AB = \begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

### 3. Verification

First, I calculate the transpose of AB.

$$
(AB)^T = \begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Now I calculate B^T A^T using row-by-column multiplication.

- Row 1, Column 1: 1x1 + 2x2 + (-1)x3 = 2
- Row 1, Column 2: 1x4 + 2x5 + (-1)x6 = 8
- Row 2, Column 1: 0x1 + 1x2 + 3x3 = 11
- Row 2, Column 2: 0x4 + 1x5 + 3x6 = 23

**Result:**

$$
B^{T} A^{T} = \begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Both results are the same.

**$(AB)^T = B^{T} A^{T}$**

This verifies that the transpose of a matrix product reverses the order of multiplication.

