
# Exercise 11 - When Do Matrices Commute?

## Question

A = [[1, 1], [0, 1]]

B = [[a, b], [c, d]]

Find the conditions for AB = BA and describe B.

## Solution

First, multiply A by B:

AB = [[a + c, b + d],
      [c, d]]

Now multiply B by A:

BA = [[a, a + b],
      [c, c + d]]

For AB = BA, the matching entries must be equal.

a + c = a, so c = 0.

b + d = a + b, so d = a.

The bottom-right entry also gives c = 0.

Therefore:

B = [[a, b],
     [0, a]]

Here a and b can be any numbers.

## Verification

Using B = [[a, b], [0, a]]:

AB = [[a, a + b], [0, a]]

BA = [[a, a + b], [0, a]]

Both results are equal.
