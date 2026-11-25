# Exercise 9 - A System from a Sum Condition

## Question

Find the numbers $x$ and $y$ that satisfy

$$
\begin{cases}
x+y=10, \\
2x+5y=32. \\
\end{cases}
$$

Solve the system and explain geometrically why the solution is unique.

## Solution

I write the augmented matrix:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}
$$

I subtract twice the first row from the second row:

$$
R_2\leftarrow R_2-2R_1
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}
$$

From the second row:

$$
3y=12,\qquad y=4
$$

Substituting $y=4$ into the first equation:

$$
x+4=10,\qquad x=6
$$

Therefore, the solution is

$$
x=6,\qquad y=4
$$

### Geometric explanation

Each original equation represents a straight line in the $xy$-plane.

The first equation can be written as

$$
y=10-x
$$

Its slope is $-1$.

The second equation can be written as

$$
y=\frac{32}{5}-\frac25x
$$

Its slope is $-\frac25$.

Since the slopes are different, the two lines are not parallel and intersect in exactly one point. The intersection point is $(6,4)$, so the system has one unique solution.

This also agrees with the coefficient-matrix determinant:

$$
\det A=1\cdot5-1\cdot2=3\neq0
$$

A nonzero determinant confirms that the system has a unique solution.

## Verification

I substitute $x=6$ and $y=4$ into both original equations.

First equation:

$$
6+4=10
$$

Second equation:

$$
2\cdot6+5\cdot4=12+20=32
$$

Both equations are satisfied. The two different slopes confirm that these lines intersect only once, at $(6,4)$.
