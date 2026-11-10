
# Exercise 5 - Row Operations

## Question

Calculate det(A) using row operations.

A = [[1, 2, 3],
     [2, 1, 0],
     [-1, 4, 2]]

Explain how each operation changes the determinant.

## Solution

I will make zeros below the main diagonal.

### Step 1

R2 = R2 - 2R1

R2 = (2, 1, 0) - (2, 4, 6)

R2 = (0, -3, -6)

The matrix becomes:

[[1, 2, 3],
 [0, -3, -6],
 [-1, 4, 2]]

### Step 2

R3 = R3 + R1

R3 = (-1, 4, 2) + (1, 2, 3)

R3 = (0, 6, 5)

The matrix becomes:

[[1, 2, 3],
 [0, -3, -6],
 [0, 6, 5]]

### Step 3

R3 = R3 + 2R2

R3 = (0, 6, 5) + (0, -6, -12)

R3 = (0, 0, -7)

The final matrix is:

[[1, 2, 3],
 [0, -3, -6],
 [0, 0, -7]]

All three row operations add a multiple of one row to another row.

These operations do not change the determinant.

The final matrix is upper triangular.

So I multiply the diagonal numbers:

det(A) = 1 * (-3) * (-7)

det(A) = 21

## Verification

Using the original matrix:

det(A) = 1 * (1 * 2 - 0 * 4)
       - 2 * (2 * 2 - 0 * (-1))
       + 3 * (2 * 4 - 1 * (-1))

= 2 - 8 + 27

= 21

Both methods give the same result.
