# Exercise 8 - Row Operations and Their Reversibility

## Question

Given the matrix:

$$
A = \begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

Perform these operations in order:

1. R2 = R2 - 2R1
2. R3 = R3 + R1
3. Swap R2 and R3

Write the matrix after each step and explain how to reverse each operation.

## Solution

### Step 1: R2 = R2 - 2R1

I multiply the first row by 2:

2R1 = (2, 4, -2)

Then I subtract it from the second row:

$R_{2} = (2, 4, 1) - (2, 4, -2)$

$R_{2} = (0, 0, 3)$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

### Step 2: R3 = R3 + R1

I add the first row to the third row:

$R_{3} = (-1, 1, 3) + (1, 2, -1)$

$R_{3} = (0, 3, 2)$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

### Step 3: Swap R2 and R3

I change the positions of the second and third rows.

The final matrix is:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

## Reversibility

Each row operation can be reversed.

1. To reverse R2 = R2 - 2R1, I use R2 = R2 + 2R1.
2. To reverse R3 = R3 + R1, I use R3 = R3 - R1.
3. To reverse swapping R2 and R3, I swap them again.

## Verification

I reverse the operations in the opposite order.

First, I swap R2 and R3 again:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

Then I subtract R1 from R3:

$R_{3} = (0, 3, 2) - (1, 2, -1) = (-1, 1, 3)$

Finally, I add 2R1 to R2:

$R_{2} = (0, 0, 3) + (2, 4, -2) = (2, 4, 1)$

I get the original matrix:

$$
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

This confirms that all three row operations are reversible.

