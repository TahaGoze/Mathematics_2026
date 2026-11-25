# Exercise 6 - A System with a Parameter

## Question

Analyze the system depending on the parameter $a$:

$$
\begin{cases}
x+y=2, \\
ax+ay=4. \\
\end{cases}
$$

Determine which of the three cases actually occur: exactly one solution, infinitely many solutions, or no solution. Give the values of $a$ for each possible case and explain why any impossible case cannot occur.

## Solution

I write the augmented matrix:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

To eliminate the first entry in the second row, I subtract $a$ times the first row:

$$
R_2 \leftarrow R_2-aR_1
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

Now I examine the value of $4-2a$.

**Case 1: $a=2$.**

In this case, $4-2a=0$, so the second row is all zeros:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Only the equation $x+y=2$ remains. One variable can be chosen freely. Let $y=t$, where $t$ is any real number. Then

$$
x=2-t,\qquad y=t,\qquad t\in\mathbb{R}
$$

Therefore, when $a=2$, the system has infinitely many solutions.

**Case 2: $a\neq2$.**

Here $4-2a\neq0$. The second row represents

$$
0x+0y=4-2a
$$

The left side is zero but the right side is not zero. This is a contradiction, so there is no solution when $a\neq2$.

**Case 3: Exactly one solution.**

This case never occurs. The two coefficient rows $(1,1)$ and $(a,a)$ are proportional for every value of $a$. The determinant of the coefficient matrix is

$$
\det A=1\cdot a-1\cdot a=0
$$

Thus, elimination can never produce two pivots for the two unknowns. The system cannot have exactly one solution.

The classification is:

- If $a=2$: infinitely many solutions.
- If $a\neq2$: no solution.
- Exactly one solution: impossible for any $a$.

## Verification

For $a=2$, substitute $x=2-t$ and $y=t$ into the original equations.

First equation:

$$
(2-t)+t=2
$$

Second equation:

$$
2(2-t)+2t=4
$$

Both equations are true for every real $t$, confirming infinitely many solutions.

For $a\neq2$, the first equation requires $x+y=2$. Multiplying this equality by $a$ gives

$$
ax+ay=2a
$$

But the second equation requires $ax+ay=4$. Both can be true only if $2a=4$, meaning $a=2$. This contradicts $a\neq2$, so there are no solutions in this case.
