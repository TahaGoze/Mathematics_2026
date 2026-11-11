# Exercise 13 - A Recurrence Written in Matrix Form

## Question

$$
F = \begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

Calculate $F^2$, $F^3$, $F^4$ and $F^5$. Compare the entries with the sequence $0,1,1,2,3,5,8,\ldots$ and describe the relationship.

Then calculate

$$
F\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

Explain how this multiplication gives the sum of two consecutive numbers and keeps one of them for the next step.

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

The top rows of $F^2$, $F^3$, $F^4$ and $F^5$ are $(2,1)$, $(3,2)$, $(5,3)$ and $(8,5)$. Each pair contains two consecutive Fibonacci numbers.

The bottom row also has consecutive Fibonacci numbers from the sequence. Each new number is the sum of the previous two numbers.

Now I multiply $F$ by the vector:

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

The multiplication changes $(a,b)$ into $(a+b,a)$. It adds the two numbers and keeps $a$ for the next step.

For the example, it adds $3+2=5$ and keeps $3$.

This is how the Fibonacci sequence works.

