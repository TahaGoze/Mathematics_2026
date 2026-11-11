# Exercise 4 - Triangular Matrix

## Question

Find the determinant without expanding:

$$
A = \begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}
$$

State the rule for any triangular matrix and explain why it works using the zero entries in this example.

## Solution

This is an upper triangular matrix because all numbers below the main diagonal are zero.

In a triangular matrix, the determinant is the product of the diagonal numbers. Here, all other terms in the determinant expansion contain a zero from below the diagonal, so only the diagonal product remains.

The diagonal numbers are:

2, -3, 7

So:

$\det(A) = 2 \cdot  (-3) \cdot  7$

$\det(A) = -42$

## Verification

The matrix is upper triangular.

The rule says to multiply all diagonal numbers.

$2 \cdot  (-3) \cdot  7 = -42$

So the determinant is -42 without expanding.

