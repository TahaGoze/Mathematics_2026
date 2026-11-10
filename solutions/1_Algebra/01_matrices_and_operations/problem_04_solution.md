# Exercise 4 - Matrix Multiplication

## Question

Given the matrices:

$$
A = \begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

1. Calculate AB.
2. Calculate BA.
3. Is AB equal to BA?

Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

$$
A = \begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

### 1. Calculate AB

I multiplied each row of A by each column of B and added the results.

- Row 1, Column 1: 1 × 2 + 2 × 3 = 8
- Row 1, Column 2: 1 × 0 + 2 × 1 = 2
- Row 2, Column 1: 0 × 2 + 1 × 3 = 3
- Row 2, Column 2: 0 × 0 + 1 × 1 = 1

**Result:**

$$
AB = \begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

### 2. Calculate BA

This time I multiplied the rows of B by the columns of A.

- Row 1, Column 1: 2 × 1 + 0 × 0 = 2
- Row 1, Column 2: 2 × 2 + 0 × 1 = 4
- Row 2, Column 1: 3 × 1 + 1 × 0 = 3
- Row 2, Column 2: 3 × 2 + 1 × 1 = 7

**Result:**

$$
BA = \begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

### 3. Comparison and Verification

AB and BA are both possible because the matrices are 2 × 2.

$$
AB = \begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

$$
BA = \begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

**AB is not equal to BA.**

I checked the calculations using row-by-column multiplication.

For example, the first entry of AB is 8, while the first entry of BA is 2.

This shows that matrix multiplication is not commutative. The order of multiplication matters.

