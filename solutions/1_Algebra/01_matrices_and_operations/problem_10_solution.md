
# Exercise 10 - Columns of a Matrix Product

## Question

A = [[1, 2, 0], [0, 1, 1]]
B = [[1, 2], [-1, 0], [3, 1]]

Find Ab1, Ab2 and AB. Explain the connection.

## Solution

The columns of B are:

b1 = [1, -1, 3]
b2 = [2, 0, 1]

First, calculate Ab1:

First row: 1(1) + 2(-1) + 0(3) = -1

Second row: 0(1) + 1(-1) + 1(3) = 2

Ab1 = [-1, 2]

Now calculate Ab2:

First row: 1(2) + 2(0) + 0(1) = 2

Second row: 0(2) + 1(0) + 1(1) = 1

Ab2 = [2, 1]

Now multiply A by B:

AB = [[-1, 2],
      [2, 1]]

## Verification and Explanation

The first column of AB is [-1, 2], which is Ab1.

The second column is [2, 1], which is Ab2.

This happens because multiplying A by B means multiplying A by each column of B.
