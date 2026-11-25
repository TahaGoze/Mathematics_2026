# Exercise 13 - Does Every Equation Add New Information?

## Question

Solve the system

$$
\begin{cases}
x_1+x_2=10, \\
x_2+x_3=8, \\
x_1-x_3=2. \\
\end{cases}
$$

Determine whether all three equations are independently necessary to describe the solution set. If an equation follows from the others, show this by calculation.

## Solution

I first check whether the third equation adds any new information.

Subtracting the second equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8
$$

The two $x_2$ terms cancel, leaving

$$
x_1-x_3=2
$$

This is exactly the third equation. Therefore, the third equation follows from the first two and is redundant. I only need the first two equations to describe the same solution set.

Now I solve

$$
\begin{cases}
x_1+x_2=10, \\
x_2+x_3=8. \\
\end{cases}
$$

There are three unknowns and only two independent equations, so I can choose one variable freely. Let

$$
x_2=t,\qquad t\in\mathbb{R}
$$

From the first equation,

$$
x_1=10-t
$$

From the second equation,

$$
x_3=8-t
$$

Thus, all solutions are

$$
\begin{pmatrix}
x_1 \\
x_2 \\
x_3 \\
\end{pmatrix} =
\begin{pmatrix}
10-t \\
t \\
8-t \\
\end{pmatrix},
\qquad t\in\mathbb{R}
$$

The system has infinitely many solutions because the parameter $t$ can be any real number.

## Verification

I check the general solution in each original equation.

First equation:

$$
(10-t)+t=10
$$

Second equation:

$$
t+(8-t)=8
$$

Third equation:

$$
(10-t)-(8-t)=2
$$

All three equations hold for every real $t$.

For a numerical check, I choose $t=3$. This gives

$$
x_1=7,\qquad x_2=3,\qquad x_3=5
$$

Substitution gives

$$
7+3=10,\qquad 3+5=8,\qquad 7-5=2
$$

This verifies the solution and confirms that the third equation does not provide an additional restriction.
