# Exercise 13 - A Recurrence Written in Matrix Form

## Question

$$
F = \begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

Calculate F^2, F^3, F^4 and F^5.

$$
Compare the results with Fibonacci numbers and calculate F \cdot  \begin{pmatrix}
a \\
b \\
\end{pmatrix}.
$$

## Solution

First, calculate the powers:

$$
F^{2} = \begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
$$

$$
F^{3} = \begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

$$
F^{4} = \begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}
$$

$$
F^{5} = \begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}
$$

The Fibonacci sequence is:

0, 1, 1, 2, 3, 5, 8, ...

I can see these numbers in the matrices.

Each new Fibonacci number is the sum of the previous two numbers.

$$
Now multiply F by \begin{pmatrix}
a \\
b \\
\end{pmatrix}:
$$

$$
F \cdot  \begin{pmatrix}
a \\
b \\
\end{pmatrix} = \begin{pmatrix}
1a + 1b \\
1a + 0b \\
\end{pmatrix}
$$

$$
F \cdot  \begin{pmatrix}
a \\
b \\
\end{pmatrix} = \begin{pmatrix}
a + b \\
a \\
\end{pmatrix}
$$

## Verification and Explanation

For example, if a = 3 and b = 2:

$$
F \cdot  \begin{pmatrix}
3 \\
2 \\
\end{pmatrix} = \begin{pmatrix}
5 \\
3 \\
\end{pmatrix}
$$

The multiplication adds 3 + 2 to make 5 and keeps 3 for the next step.

This is how the Fibonacci sequence works.
