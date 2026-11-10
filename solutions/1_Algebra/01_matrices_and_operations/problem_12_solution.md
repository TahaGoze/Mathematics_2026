# Exercise 12 - Formula for a Matrix Power

## Question

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

Calculate A^2, A^3 and A^4. Find a formula for A^n and prove it.

## Solution

$A^{2} = A \cdot  A$

$$
A^{2} = \begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

$A^{3} = A^{2} \cdot  A$

$$
A^{3} = \begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}
$$

$A^{4} = A^{3} \cdot  A$

$$
A^{4} = \begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}
$$

The top-right number increases by 1 each time.

So my formula is:

$$
A^{n} = \begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
$$

## Verification

First, the formula works for n = 1.

Now assume:

$$
A^{n} = \begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
$$

Multiply by A:

$A^{n+1} = A^{n} \cdot  A$

$$
= \begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix} \cdot  \begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

$$
= \begin{pmatrix}
1 & n + 1 \\
0 & 1 \\
\end{pmatrix}
$$

This is the same formula with n + 1.

So the formula works for all positive integers n.

