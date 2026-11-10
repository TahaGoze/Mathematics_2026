
# Exercise 9 - Composing Transformations

## Question

Given:

S = [[2, 0], [0, 1]]

R = [[0, -1], [1, 0]]

x = [1, 2]

Calculate RSx and SRx. Compare the results and explain why the order matters.

## Solution

### 1. Calculate RSx

First, I calculate Sx:

Sx = [[2, 0], [0, 1]] * [1, 2]

First row: 2 * 1 + 0 * 2 = 2

Second row: 0 * 1 + 1 * 2 = 2

Sx = [2, 2]

Now I multiply by R:

RSx = [[0, -1], [1, 0]] * [2, 2]

First row: 0 * 2 + (-1) * 2 = -2

Second row: 1 * 2 + 0 * 2 = 2

RSx = [-2, 2]

### 2. Calculate SRx

First, I calculate Rx:

Rx = [[0, -1], [1, 0]] * [1, 2]

First row: 0 * 1 + (-1) * 2 = -2

Second row: 1 * 1 + 0 * 2 = 1

Rx = [-2, 1]

Now I multiply by S:

SRx = [[2, 0], [0, 1]] * [-2, 1]

First row: 2 * (-2) + 0 * 1 = -4

Second row: 0 * (-2) + 1 * 1 = 1

SRx = [-4, 1]

## Comparison and Explanation

RSx = [-2, 2]

SRx = [-4, 1]

The results are different.

S makes the horizontal coordinate 2 times bigger.
R rotates the vector 90 degrees counterclockwise.

In RSx, I first scale the vector and then rotate it.

In SRx, I first rotate the vector and then scale it.

The order matters because rotation changes the direction of the vector before or after scaling.

## Verification

I calculated both results using matrix-vector multiplication.

RSx = [-2, 2] and SRx = [-4, 1].

Since the results are not equal, the order of these transformations matters.
