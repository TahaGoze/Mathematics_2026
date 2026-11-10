# Exercise 3 - Swapping Two Rows

## Question

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

Calculate det(A).

Then swap the first and second rows to make B. Predict and verify det(B).

## Solution

First, calculate det(A) using the first row:

$\det(A) = 1 \cdot  (3 \cdot  1 - 1 \cdot  1)$
       - 2 * (0 * 1 - 1 * 2)

= 1 * 2 - 2 * (-2)

= 2 + 4

$\det(A) = 6$

Now swap the first and second rows.

$$
B = \begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

Swapping two rows changes the sign of the determinant.

So I predict:

$\det(B) = -6$

## Verification

Calculate det(B) using the first row:

$\det(B) = -3 \cdot  (1 \cdot  1 - 0 \cdot  2)$
       + 1 * (1 * 1 - 2 * 2)

$= -3 + (1 - 4)$

$= -3 - 3$

$\det(B) = -6$

This confirms the prediction.
