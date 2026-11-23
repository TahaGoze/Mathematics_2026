# Exercise 10 - Detecting Dependence

## Question

Without a full determinant calculation, explain why

$$
\det\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0
$$

Identify which rows depend on each other and explain what this means for invertibility.

## Solution

The first row is:

$$
R_1=(1,2,3)
$$

The second row is:

$$
R_2=(2,4,6)=2R_1
$$

So the second row is twice the first row.

When two rows are dependent, the determinant is zero.

Therefore:

$$
\det A=0
$$

A square matrix with determinant zero is not invertible.

## Verification

The row operation $R_2\leftarrow R_2-2R_1$ makes the second row $(0,0,0)$.

A matrix with a zero row has determinant zero. This confirms the result without expanding the determinant.
