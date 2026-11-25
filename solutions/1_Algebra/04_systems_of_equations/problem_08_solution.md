# Exercise 8 - Two Systems with the Same Coefficient Matrix

## Question

Solve both systems using elimination.

**System 1:**

$$
\begin{cases}
2x+y=5, \\
x-y=1. \\
\end{cases}
$$

**System 2:**

$$
\begin{cases}
2x+y=1, \\
x-y=4. \\
\end{cases}
$$

Compare the successive elimination steps. Identify which part of the calculation is the same in both systems and explain why.

## Solution

### System 1

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

I swap the rows to obtain a leading coefficient of $1$:

$$
R_1\leftrightarrow R_2
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

I subtract twice the first row from the second:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

The second row gives $3y=3$, so $y=1$.

The first row gives $x-y=1$, so

$$
x=1+y=2
$$

Thus, System 1 has the solution

$$
x=2,\qquad y=1
$$

### System 2

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$

I apply the same row swap:

$$
R_1\leftrightarrow R_2
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

I apply the same elimination step:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

The second row gives

$$
3y=-7,\qquad y=-\frac73
$$

The first row gives $x-y=4$. Substituting $y=-\frac73$:

$$
x=4+y=4-\frac73=\frac53
$$

Thus, System 2 has the solution

$$
x=\frac53,\qquad y=-\frac73
$$

### Comparison of the elimination steps

Both systems have the same coefficient matrix:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix}
$$

Therefore, both use the same row swap followed by the same operation $R_2\leftarrow R_2-2R_1$. In both cases, the coefficient rows become $(1,-1)$ and $(0,3)$.

Only the right-hand sides change. For System 1, the new second right-hand side is

$$
5-2\cdot1=3
$$

For System 2, it is

$$
1-2\cdot4=-7
$$

The same elimination pattern and pivot coefficient $3$ can be reused because $A$ is unchanged. Different right-hand sides lead to different values of $y$ and $x$.

## Verification

For System 1, substitute $x=2$ and $y=1$:

$$
2\cdot2+1=5
$$

$$
2-1=1
$$

Both equations hold.

For System 2, substitute $x=\frac53$ and $y=-\frac73$:

$$
2\cdot\frac53-\frac73=\frac{10-7}{3}=1
$$

$$
\frac53-\left(-\frac73\right)=\frac{12}{3}=4
$$

Both equations hold, so the two solutions and the repeated elimination steps are correct.
