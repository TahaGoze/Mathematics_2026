# Exercise 3 - Inconsistent System

## Question

Solve the system or show that it is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7. \\
\end{cases}
$$

Use elimination to show where the contradiction appears in the augmented matrix. Explain what the contradiction means for the original equations.

## Solution

First, I write the augmented matrix of the system:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

I subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2-2R_1
$$

The second row becomes

$$
(2,4,7)-2(1,2,3)=(0,0,1)
$$

So the augmented matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row represents the equation

$$
0x+0y=1
$$

This means $0=1$, which is impossible. Therefore, the system is inconsistent and has no solution.

## Verification

The first equation says $x+2y=3$.

If I multiply both sides by $2$, I get

$$
2x+4y=6
$$

However, the second original equation requires

$$
2x+4y=7
$$

The same expression cannot equal both $6$ and $7$. This confirms the contradiction found by elimination and shows that there is no pair $(x,y)$ satisfying both equations.
