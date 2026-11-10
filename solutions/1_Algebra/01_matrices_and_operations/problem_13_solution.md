
# Exercise 13 - A Recurrence Written in Matrix Form

## Question

F = [[1, 1], [1, 0]]

Calculate F^2, F^3, F^4 and F^5.

Compare the results with Fibonacci numbers and calculate F * [a, b].

## Solution

First, calculate the powers:

F^2 = [[2, 1], [1, 1]]

F^3 = [[3, 2], [2, 1]]

F^4 = [[5, 3], [3, 2]]

F^5 = [[8, 5], [5, 3]]

The Fibonacci sequence is:

0, 1, 1, 2, 3, 5, 8, ...

I can see these numbers in the matrices.

Each new Fibonacci number is the sum of the previous two numbers.

Now multiply F by [a, b]:

F * [a, b] = [1a + 1b, 1a + 0b]

F * [a, b] = [a + b, a]

## Verification and Explanation

For example, if a = 3 and b = 2:

F * [3, 2] = [5, 3]

The multiplication adds 3 + 2 to make 5 and keeps 3 for the next step.

This is how the Fibonacci sequence works.
