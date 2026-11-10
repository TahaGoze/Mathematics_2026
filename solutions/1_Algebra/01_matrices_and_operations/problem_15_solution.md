# Exercise 15 - Associativity of Multiplication

## Question

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

$$
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

$$
C = \begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}
$$

Calculate (AB)C and A(BC). Compare the results and explain associativity.

## Solution

### First method: (AB)C

First, calculate AB:

$$
AB = \begin{pmatrix}
1(1)+2(2)+0(-1) & 1(0)+2(1)+0(3) \\
0(1)+1(2)+1(-1) & 0(0)+1(1)+1(3) \\
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

Now multiply by C:

$$
(AB)C = \begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix} \cdot  \begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}
$$

$$
(AB)C = \begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

### Second method: A(BC)

First, calculate BC:

$$
BC = \begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}
$$

Now multiply A by BC:

$$
A(BC) = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix} \cdot 
        \begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}
$$

$$
A(BC) = \begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

## Verification and Explanation

Both methods give the same matrix:

$$
(AB)C = A(BC) = \begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

This is called associativity.

It means we can change the grouping of multiplication without changing the result.

The first method uses 20 number multiplications.
The second method uses 24 number multiplications.

So calculating AB first is a little shorter in this example.
