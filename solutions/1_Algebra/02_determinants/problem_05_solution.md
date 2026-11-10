# Exercise 5 - Row Operations

## Question

Calculate det(A) using row operations.

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

Explain how each operation changes the determinant.

## Solution

I will make zeros below the main diagonal.

### Step 1

$R_{2} = R_{2} - 2R1$

$R_{2} = (2, 1, 0) - (2, 4, 6)$

$R_{2} = (0, -3, -6)$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

### Step 2

$R_{3} = R_{3} + R_{1}$

$R_{3} = (-1, 4, 2) + (1, 2, 3)$

$R_{3} = (0, 6, 5)$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

### Step 3

$R_{3} = R_{3} + 2R2$

$R_{3} = (0, 6, 5) + (0, -6, -12)$

$R_{3} = (0, 0, -7)$

The final matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

All three row operations add a multiple of one row to another row.

These operations do not change the determinant.

The final matrix is upper triangular.

So I multiply the diagonal numbers:

$\det(A) = 1 \cdot  (-3) \cdot  (-7)$

$\det(A) = 21$

## Verification

Using the original matrix:

$\det(A) = 1 \cdot  (1 \cdot  2 - 0 \cdot  4)$
       - 2 * (2 * 2 - 0 * (-1))
       + 3 * (2 * 4 - 1 * (-1))

= 2 - 8 + 27

= 21

Both methods give the same result.

