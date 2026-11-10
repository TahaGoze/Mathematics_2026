# Exercise 7 - Identity Matrix, Zero Matrix, and Powers

## Question

Given:

$$
A = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

Calculate AI, IA, A + 0, A^2 and A^3.

Explain the roles of I and 0, and describe the pattern in the powers of A.

## Solution

### 1. AI, IA and A + 0

The identity matrix is:

$$
I = \begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Multiplying A by I does not change A.

$$
AI = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
IA = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

The zero matrix is:

$$
0 = \begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
$$

Adding zero does not change the matrix.

$$
A + 0 = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

### 2. Calculate A^2

A^2 means A multiplied by A.

I multiplied the rows of A by the columns of A.

- Row 1, Column 1: 2 x 2 + 1 x 0 = 4
- Row 1, Column 2: 2 x 1 + 1 x 2 = 4
- Row 2, Column 1: 0 x 2 + 2 x 0 = 0
- Row 2, Column 2: 0 x 1 + 2 x 2 = 4

**Result:**

$$
A^{2} = \begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

### 3. Calculate A^3

$A^{3} = A^{2} x A$

I used the same row-by-column multiplication.

- Row 1, Column 1: 4 x 2 + 4 x 0 = 8
- Row 1, Column 2: 4 x 1 + 4 x 2 = 12
- Row 2, Column 1: 0 x 2 + 4 x 0 = 0
- Row 2, Column 2: 0 x 1 + 4 x 2 = 8

**Result:**

$$
A^{3} = \begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

### 4. Pattern

Comparing the matrices:

$$
A = \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
A^{2} = \begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

$$
A^{3} = \begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

The diagonal numbers double each time: 2, 4, 8.

The bottom-left entry always stays 0.

The top-right entry changes from 1 to 4 to 12.

## Verification

I checked A^2 by multiplying A by itself.

I also checked A^3 by multiplying A^2 by A.

Both calculations follow the row-by-column multiplication rule.

AI = IA = A and A + 0 = A, as expected.

This shows that I is the identity matrix for multiplication and 0 is the identity matrix for addition.

