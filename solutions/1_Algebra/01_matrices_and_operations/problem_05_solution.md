
# Exercise 5 - Matrix Times Vector

## Question

Given:

A = [[2, -1], [1, 3]]

x = [4, 2]

1. Calculate Ax.
2. Express Ax as a linear combination of the columns of A.

## Solution

### 1. Calculate Ax

I multiplied each row of A by vector x.

- First row: 2 x 4 + (-1) x 2 = 6
- Second row: 1 x 4 + 3 x 2 = 10

**Result:**

Ax = [6, 10]

### 2. Linear Combination

The columns of A are:

- First column: [2, 1]
- Second column: [-1, 3]

Using the numbers 4 and 2 from vector x:

4 x [2, 1] + 2 x [-1, 3]

= [8, 4] + [-2, 6]

= [6, 10]

### Verification

Both methods give the same result: [6, 10].

So the calculation is correct.
    
