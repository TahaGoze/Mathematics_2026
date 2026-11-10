# Exercise 2 - Determinant of a 3x3 Matrix

## Question

$$
A = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

Calculate det(A) using Sarrus' rule and check the result.

## Solution

Using Sarrus' rule, first calculate the downward diagonals:

$1 \cdot  3 \cdot  5 = 15$

$2 \cdot  4 \cdot  2 = 16$

$(-1) \cdot  0 \cdot  1 = 0$

$Total = 15 + 16 + 0 = 31$

Now calculate the upward diagonals:

$(-1) \cdot  3 \cdot  2 = -6$

$2 \cdot  0 \cdot  5 = 0$

$1 \cdot  4 \cdot  1 = 4$

$Total = -6 + 0 + 4 = -2$

Subtract the totals:

$\det(A) = 31 - (-2)$

$\det(A) = 33$

## Verification

I use the row operation:

$R_{3} = R_{3} - 2R1$

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}
$$

This row operation does not change the determinant.

Using the first column:

$\det(A) = 1 \cdot  (3 \cdot  7 - 4 \cdot  (-3))$

= 21 + 12

= 33

Both methods give the same result.
