
# Exercise 12 - Formula for a Matrix Power

## Question

A = [[1, 1], [0, 1]]

Calculate A^2, A^3 and A^4. Find a formula for A^n and prove it.

## Solution

A^2 = A * A

A^2 = [[1, 2], [0, 1]]

A^3 = A^2 * A

A^3 = [[1, 3], [0, 1]]

A^4 = A^3 * A

A^4 = [[1, 4], [0, 1]]

The top-right number increases by 1 each time.

So my formula is:

A^n = [[1, n], [0, 1]]

## Verification

First, the formula works for n = 1.

Now assume:

A^n = [[1, n], [0, 1]]

Multiply by A:

A^(n+1) = A^n * A

= [[1, n], [0, 1]] * [[1, 1], [0, 1]]

= [[1, n + 1], [0, 1]]

This is the same formula with n + 1.

So the formula works for all positive integers n.
