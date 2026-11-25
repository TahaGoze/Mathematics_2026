# Exercise 13 - Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways: first calculate $T$ and then its inverse, and then use the property $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Also calculate $H^{-1}S^{-1}$, show that this incorrect order gives a different matrix, and explain why a composition must be undone in reverse order.

## Solution

### 1. Calculate T and then its inverse

First, I multiply $H$ by $S$:

$$
T=HS=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Multiplying the rows and columns gives

$$
T=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

The determinant is

$$
\det T=2\cdot1-1\cdot0=2
$$

Since the determinant is not zero, $T$ is invertible. Using the formula for a 2x2 matrix, I get

$$
T^{-1}=
\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}
$$

Therefore,

$$
T^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
$$

### 2. Use the inverse-of-a-product property

The inverse matrices are

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

The inverse of a product reverses the order of its factors:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

Now I multiply in that order:

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

This gives

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
$$

Both methods give the same inverse.

### 3. Check the incorrect order

If I multiply the inverse matrices in the original order, the result is

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

So

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

This is different from $T^{-1}$ because the top-right entry is $-1$ instead of $-\frac12$.

For column vectors, $T=HS$ first applies the scaling $S$ and then the shear $H$. To return to the original vector, I must undo the shear with $H^{-1}$ first and then undo the scaling with $S^{-1}$. This is why the inverse is $S^{-1}H^{-1}$, not $H^{-1}S^{-1}$.

## Verification

I check the correct inverse by multiplication:

$$
TT^{-1}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
$$

The product is

$$
TT^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I
$$

The incorrect order does not give the identity matrix:

$$
T(H^{-1}S^{-1})=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

This product is

$$
T(H^{-1}S^{-1})=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Therefore, only $S^{-1}H^{-1}$ is the inverse of $T$.
