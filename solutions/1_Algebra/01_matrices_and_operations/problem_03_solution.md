# Exercise 3 - Matrix Multiplication

## Question

Given the matrix sizes:

- A: 2 x 3
- B: 3 x 4
- C: 4 x 2
- D: 2 x 2

Determine whether the following matrix products are defined:

AB, BA, BC, CB, AC, CA, AD, DA

If a product is defined, state the size of the result.

Justify each answer using the dimension compatibility rule.

## Solution

## Rule

Matrix multiplication is possible when the number of columns of the first matrix equals the number of rows of the second matrix.

## Solutions

- AB: (2x3)(3x4) -> 2x4 (Defined)
- BA: (3x4)(2x3) -> Undefined (4 != 2)
- BC: (3x4)(4x2) -> 3x2 (Defined)
- CB: (4x2)(3x4) -> Undefined (2 != 3)
- AC: (2x3)(4x2) -> Undefined (3 != 4)
- CA: (4x2)(2x3) -> 4x3 (Defined)
- AD: (2x3)(2x2) -> Undefined (3 != 2)
- DA: (2x2)(2x3) -> 2x3 (Defined)

## Verification

All products were checked using the dimension compatibility rule.
