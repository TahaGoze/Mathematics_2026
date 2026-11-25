# Exercise 10 - A Polynomial Through Three Points

## Question

Find the polynomial

$$
p(x)=ax^2+bx+c
$$

whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$.

Reduce the problem to a system of equations, solve for the coefficients $a$, $b$, and $c$, and verify the result by substituting all three given points.

## Solution

For the graph to pass through $(0,1)$, $(1,3)$, and $(2,9)$, the polynomial must satisfy

$$
p(0)=1,\qquad p(1)=3,\qquad p(2)=9
$$

Substituting each value of $x$ into $p(x)=ax^2+bx+c$ gives

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9. \\
\end{cases}
$$

This is a linear system for the unknown coefficients $a$, $b$, and $c$. In augmented matrix form, it is

$$
\begin{pmatrix}
0 & 0 & 1 & \mid & 1 \\
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
\end{pmatrix}
$$

The first equation immediately gives $c=1$.

Using $c=1$ in the other two equations:

$$
\begin{cases}
a+b=2, \\
4a+2b=8. \\
\end{cases}
$$

Divide the second equation by $2$:

$$
2a+b=4
$$

Subtract the equation $a+b=2$ from $2a+b=4$:

$$
(2a+b)-(a+b)=4-2
$$

Therefore, $a=2$. Substituting into $a+b=2$ gives

$$
2+b=2,\qquad b=0
$$

The coefficients are

$$
a=2,\qquad b=0,\qquad c=1
$$

Thus, the required polynomial is

$$
p(x)=2x^2+1
$$

## Verification

Check each of the three given points.

For $(0,1)$:

$$
p(0)=2\cdot0^2+1=1
$$

For $(1,3)$:

$$
p(1)=2\cdot1^2+1=3
$$

For $(2,9)$:

$$
p(2)=2\cdot2^2+1=9
$$

The polynomial gives the required value at all three points. Also, the three independent equations determine $a$, $b$, and $c$ uniquely, so this is the only polynomial of the given form passing through these points.
