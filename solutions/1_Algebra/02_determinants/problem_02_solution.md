
# Exercise 2 - Determinant of a 3x3 Matrix

## Question

A = [[1, 2, -1],
     [0, 3, 4],
     [2, 1, 5]]

Calculate det(A) using Sarrus' rule and check the result.

## Solution

Using Sarrus' rule, first calculate the downward diagonals:

1 * 3 * 5 = 15

2 * 4 * 2 = 16

(-1) * 0 * 1 = 0

Total = 15 + 16 + 0 = 31

Now calculate the upward diagonals:

(-1) * 3 * 2 = -6

2 * 0 * 5 = 0

1 * 4 * 1 = 4

Total = -6 + 0 + 4 = -2

Subtract the totals:

det(A) = 31 - (-2)

det(A) = 33

## Verification

I use the row operation:

R3 = R3 - 2R1

The new matrix is:

[[1, 2, -1],
 [0, 3, 4],
 [0, -3, 7]]

This row operation does not change the determinant.

Using the first column:

det(A) = 1 * (3 * 7 - 4 * (-3))

= 21 + 12

= 33

Both methods give the same result.
