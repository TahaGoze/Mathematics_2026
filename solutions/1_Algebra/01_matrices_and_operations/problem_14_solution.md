# Exercise 14 - Rotation Matrices

## Question

The rotation matrix is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}
$$

Calculate $R(\alpha)R(\beta)$ and use the sine and cosine angle-sum formulas to show that it equals $R(\alpha+\beta)$. Explain the result geometrically.

## Solution

First, multiply the two matrices:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & -\sin\alpha\sin\beta+\cos\alpha\cos\beta \\
\end{pmatrix}
$$

I use the angle-sum formulas:

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

So the product is

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
=R(\alpha+\beta)
$$

## Verification and Explanation

Geometrically, rotating by $\beta$ and then by $\alpha$ means rotating by the total angle $\alpha+\beta$.

For example, two rotations of $90^\circ$ give a rotation of $180^\circ$.

This agrees with the matrix result.

