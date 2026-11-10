# Exercise 11 - When Do Matrices Commute?

## Question

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

Find the conditions for AB = BA and describe B.

## Solution

First, multiply A by B:

$$
AB = \begin{pmatrix}
a + c & b + d \\
c & d \\
\end{pmatrix}
$$

Now multiply B by A:

$$
BA = \begin{pmatrix}
a & a + b \\
c & c + d \\
\end{pmatrix}
$$

For AB = BA, the matching entries must be equal.

a + c = a, so c = 0.

b + d = a + b, so d = a.

The bottom-right entry also gives c = 0.

Therefore:

$$
B = \begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}
$$

Here a and b can be any numbers.

## Verification

Using this matrix:

$$
B = \begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
a & a + b \\
0 & a \\
\end{pmatrix}
$$

$$
BA = \begin{pmatrix}
a & a + b \\
0 & a \\
\end{pmatrix}
$$

Both results are equal.

