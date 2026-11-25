# Exercise 12 - Finding Inverses Without Starting from Scratch

## Question

It is given that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Without finding $A$, calculate $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each answer using the appropriate inverse property.

## Solution

### 1. Inverse of 3A

For a nonzero scalar $c$, the inverse property is

$$
(cA)^{-1}=\frac{1}{c}A^{-1}
$$

Since $c=3$, I multiply every entry of $A^{-1}$ by $\frac13$:

$$
(3A)^{-1}=
\frac13
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Therefore,

$$
(3A)^{-1}=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix}
$$

### 2. Inverse of the transpose

The inverse of a transpose is the transpose of the inverse:

$$
(A^T)^{-1}=(A^{-1})^T
$$

I transpose the given inverse by exchanging its rows and columns:

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}
$$

### 3. Inverse of A squared

The inverse of a product reverses the order of the factors. Since $A^2=AA$, I have

$$
(A^2)^{-1}=(AA)^{-1}=A^{-1}A^{-1}
$$

I multiply the given inverse matrix by itself:

$$
(A^2)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Multiplying rows by columns gives

$$
(A^2)^{-1}=
\begin{pmatrix}
2\cdot2+(-1)\cdot(-3) & 2\cdot(-1)+(-1)\cdot2 \\
(-3)\cdot2+2\cdot(-3) & (-3)\cdot(-1)+2\cdot2 \\
\end{pmatrix}
$$

So the result is

$$
(A^2)^{-1}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}
$$

## Verification

The three inverse properties can be checked from $AA^{-1}=A^{-1}A=I$.

For the scalar multiple:

$$
(3A)\left(\frac13 A^{-1}\right)=AA^{-1}=I
$$

For the transpose:

$$
A^T(A^{-1})^T=(A^{-1}A)^T=I
$$

For the square:

$$
A^2(A^{-1}A^{-1})=A(AA^{-1})A^{-1}=I
$$

Each product gives the identity matrix. This verifies the methods without calculating $A$ itself.
