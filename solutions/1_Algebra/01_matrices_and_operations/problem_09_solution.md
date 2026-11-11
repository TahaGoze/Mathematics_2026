# Exercise 9 - Composing Transformations

## Question

Given:

$$
S = \begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

$$
R = \begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
$$

$$
x = \begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

Here $S$ describes nonuniform scaling (it doubles the horizontal coordinate), and $R$ describes a $90^\circ$ counterclockwise rotation.

Calculate $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

### 1. Calculate RSx

First, I calculate Sx:

$$
Sx = \begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix} \cdot  \begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

First row: $2 \cdot  1 + 0 \cdot  2 = 2$

Second row: $0 \cdot  1 + 1 \cdot  2 = 2$

$$
Sx = \begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

Now I multiply by R:

$$
RSx = \begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix} \cdot  \begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

First row: $0 \cdot  2 + (-1) \cdot  2 = -2$

Second row: $1 \cdot  2 + 0 \cdot  2 = 2$

$$
RSx = \begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

### 2. Calculate SRx

First, I calculate Rx:

$$
Rx = \begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix} \cdot  \begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

First row: $0 \cdot  1 + (-1) \cdot  2 = -2$

Second row: $1 \cdot  1 + 0 \cdot  2 = 1$

$$
Rx = \begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

Now I multiply by S:

$$
SRx = \begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix} \cdot  \begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

First row: $2 \cdot  (-2) + 0 \cdot  1 = -4$

Second row: $0 \cdot  (-2) + 1 \cdot  1 = 1$

$$
SRx = \begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

## Comparison and Explanation

$$
RSx = \begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

$$
SRx = \begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

The results are different.

S makes the horizontal coordinate 2 times bigger.
R rotates the vector 90 degrees counterclockwise.

In RSx, I first scale the vector and then rotate it.

In SRx, I first rotate the vector and then scale it.

The order matters because rotation changes the direction of the vector before or after scaling.

## Verification

I checked both vectors using matrix-vector multiplication.

The final vectors are different, so $RSx\neq SRx$. This confirms that the order matters.
