# Exercise 2

## 1. Matrix Addition (A+B)

Both matrices have the same size (2x2), so addition is possible.

We add the corresponding entries of the matrices.

Matrices of different sizes cannot be added because their corresponding entries do not match in position.

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
$$

### Verification

We can verify the result by subtracting B from A+B.

$$
(A+B)-B=
\begin{pmatrix}
5-4 & 0-(-2) \\
-1-0 & 8-5
\end{pmatrix}
=
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix}
=A
$$

The result is correct.

## 2. Matrix Subtraction (A-B)

Both matrices have the same size (2x2), so subtraction is possible.

We subtract the corresponding entries.

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
$$

### Verification

We can verify the result by adding B to A-B.

$$
(A-B)+B=
\begin{pmatrix}
-3+4 & 4+(-2) \\
-1+0 & -2+5
\end{pmatrix}
=
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix}
=A
$$

The result is correct.

## 3. Scalar Multiplication and Subtraction (3A-2B)

First, we multiply every entry of A by 3 and every entry of B by 2.

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix}
$$

$$
2B=
\begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}
$$

Both matrices have the same size (2x2), so subtraction is possible.

We subtract the corresponding entries.

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
$$

### Verification

We can verify the result by adding 2B to 3A-2B.

$$
(3A-2B)+2B=
\begin{pmatrix}
-5+8 & 10+(-4) \\
-3+0 & -1+10
\end{pmatrix}
=
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix}
=3A
$$

The result is correct.
    
