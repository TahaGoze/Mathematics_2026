
# Exercise 15 - Associativity of Multiplication

## Question

A = [[1, 2, 0], [0, 1, 1]]

B = [[1, 0], [2, 1], [-1, 3]]

C = [[2, 1], [0, -1]]

Calculate (AB)C and A(BC). Compare the results and explain associativity.

## Solution

### First method: (AB)C

First, calculate AB:

AB = [[1(1)+2(2)+0(-1), 1(0)+2(1)+0(3)],
      [0(1)+1(2)+1(-1), 0(0)+1(1)+1(3)]]

AB = [[5, 2], [1, 4]]

Now multiply by C:

(AB)C = [[5, 2], [1, 4]] * [[2, 1], [0, -1]]

(AB)C = [[10, 3], [2, -3]]

### Second method: A(BC)

First, calculate BC:

BC = [[2, 1],
      [4, 1],
      [-2, -4]]

Now multiply A by BC:

A(BC) = [[1, 2, 0], [0, 1, 1]] *
        [[2, 1], [4, 1], [-2, -4]]

A(BC) = [[10, 3], [2, -3]]

## Verification and Explanation

Both methods give the same matrix:

(AB)C = A(BC) = [[10, 3], [2, -3]]

This is called associativity.

It means we can change the grouping of multiplication without changing the result.

The first method uses 20 number multiplications.
The second method uses 24 number multiplications.

So calculating AB first is a little shorter in this example.
