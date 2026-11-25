# Exercise 15 - Classifying Three Systems

## Question

For each of the following systems, use only as much Gaussian elimination as needed to determine whether it has exactly one solution, infinitely many solutions, or no solution. Explain the classification for each system.

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0. \\
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4. \\
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5. \\
\end{cases}
$$

## Solution

### System 1 - Exactly one solution

I write the augmented matrix:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Subtract the first row from the second:

$$
R_2\leftarrow R_2-R_1
$$

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

The second row gives $-2y=-2$, so $y=1$. The first row then gives $x+1=2$, so $x=1$.

There is a pivot in each unknown's column. Therefore, the system has exactly one solution:

$$
(x,y)=(1,1)
$$

### System 2 - Infinitely many solutions

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Subtract twice the first row from the second:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row is $0=0$, so it adds no new condition. The first equation is the only restriction.

Let $y=t$, where $t$ can be any real number. Then

$$
x=2-t,\qquad y=t,\qquad t\in\mathbb{R}
$$

Since $t$ is free, System 2 has infinitely many solutions.

### System 3 - No solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Subtract twice the first row from the second:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row says $0=1$, which is impossible. Therefore, System 3 is inconsistent and has no solution.

## Verification

**System 1:** Substitute $(x,y)=(1,1)$ into both equations:

$$
1+1=2
$$

$$
1-1=0
$$

Both are true.

**System 2:** Substitute the general solution $x=2-t$ and $y=t$:

$$
(2-t)+t=2
$$

$$
2(2-t)+2t=4
$$

Both hold for every real $t$, confirming infinitely many solutions.

**System 3:** The first equation requires $x+y=2$. Multiplying it by $2$ gives $2x+2y=4$, but the second equation requires $2x+2y=5$. They cannot both be true, confirming that no solution exists.

The three systems illustrate the three possible classifications: exactly one solution, infinitely many solutions, and no solution.
