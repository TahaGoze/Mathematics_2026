# Exercise 15 - Two Methods for Solving the Same System

## Question

Given

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

and

$$
b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways: (1) using $x=A^{-1}b$, and (2) using Gaussian elimination. Compare the answers and the number of essential steps, and state which method is simpler in this example.

## Solution

### 1. Using the inverse matrix

First, I calculate the determinant of $A$:

$$
\det A=2\cdot3-1\cdot1=5
$$

Since the determinant is not zero, $A^{-1}$ exists. The formula for a 2x2 matrix gives

$$
A^{-1}=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

To find $x$, I multiply $A^{-1}$ by $b$:

$$
x=A^{-1}b=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

The entries are $3\cdot7-1\cdot8=13$ and $-1\cdot7+2\cdot8=9$.

Therefore,

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

### 2. Using Gaussian elimination

The system is

$$
2x_1+x_2=7
$$

$$
x_1+3x_2=8
$$

I write its augmented matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

First, I swap the rows to get a leading entry of $1$:

$$
R_1\leftrightarrow R_2
$$

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

Next, I subtract twice the first row from the second row:

$$
R_2\leftarrow R_2-2R_1
$$

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

The second row gives $-5x_2=-9$, so

$$
x_2=\frac95
$$

I substitute this into the first equation:

$$
x_1+3\cdot\frac95=8
$$

$$
x_1=8-\frac{27}{5}=\frac{13}{5}
$$

Therefore, Gaussian elimination gives

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

### 3. Comparison

Both methods give exactly the same solution.

The inverse method has three main calculation steps: finding the determinant, finding the inverse matrix, and multiplying the inverse by $b$.

The Gaussian elimination method uses two row operations (one swap and one elimination), followed by back-substitution to find the two unknowns.

For this single small system, Gaussian elimination is slightly simpler because I do not need to calculate the whole inverse matrix. The inverse method can be useful if I need to solve several systems with the same matrix $A$ but different vectors $b$.

## Verification

I substitute the solution into the original equation $Ax=b$:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

The first entry is

$$
2\cdot\frac{13}{5}+\frac95=\frac{26+9}{5}=7
$$

The second entry is

$$
\frac{13}{5}+3\cdot\frac95=\frac{13+27}{5}=8
$$

Thus,

$$
Ax=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
=b
$$

Both methods solve the original system correctly.
