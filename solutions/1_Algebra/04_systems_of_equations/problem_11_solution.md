# Exercise 11 - A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on the parameter $t$ for the system

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3. \\
\end{cases}
$$

Use Gaussian elimination. Separately examine parameter values at which the standard calculation would require division by zero.

## Solution

First, I write the augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

I eliminate the first entries in rows 2 and 3:

$$
R_2\leftarrow R_2-R_1
$$

$$
R_3\leftarrow R_3-R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

The last two rows give

$$
(t-1)y=1
$$

$$
(t-1)z=2
$$

I must consider separately whether $t-1$ is zero.

### Case 1: $t\neq1$

Since $t-1\neq0$, I can divide the last two equations by $t-1$:

$$
y=\frac{1}{t-1},\qquad z=\frac{2}{t-1}
$$

Using the first equation $x+y+z=1$,

$$
x=1-\frac{1}{t-1}-\frac{2}{t-1}
$$

Simplifying gives

$$
x=\frac{t-4}{t-1}
$$

Therefore, the only solution for $t\neq1$ is

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
\frac{t-4}{t-1} \\
\frac{1}{t-1} \\
\frac{2}{t-1} \\
\end{pmatrix}
$$

All three variable columns have a pivot, so the solution is unique.

### Case 2: $t=1$

If $t=1$, the eliminated matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & 0 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 2 \\
\end{pmatrix}
$$

The second row requires $0=1$ and the third requires $0=2$. Both are impossible. Therefore, the system has no solution when $t=1$.

There is no parameter value with infinitely many solutions: $t\neq1$ gives three pivots, and $t=1$ produces contradictions.

## Verification

For $t\neq1$, I substitute the proposed solution into each original equation.

First equation:

$$
x+y+z=\frac{t-4+1+2}{t-1}=\frac{t-1}{t-1}=1
$$

Second equation:

$$
x+ty+z=\frac{t-4+t+2}{t-1}=\frac{2t-2}{t-1}=2
$$

Third equation:

$$
x+y+tz=\frac{t-4+1+2t}{t-1}=\frac{3t-3}{t-1}=3
$$

All three equations are satisfied whenever $t\neq1$.

For $t=1$, the original left-hand sides all become $x+y+z$, but the right-hand sides are $1$, $2$, and $3$. One expression cannot equal three different numbers, confirming that no solution exists.

The final classification is: exactly one solution if $t\neq1$, no solution if $t=1$, and infinitely many solutions for no value of $t$.
