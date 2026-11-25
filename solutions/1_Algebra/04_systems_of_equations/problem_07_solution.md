# Exercise 7 - Choosing a Method Deliberately

## Question

Choose a suitable method for each situation, considering the structure of the matrix and the number of right-hand sides.

**Case 1:** Solve the following system with a triangular coefficient matrix completely:

$$
\begin{cases}
2x-y=3, \\
4y=8. \\
\end{cases}
$$

**Case 2:** There are three systems $Ax=b_i$, for $i=1,2,3$, with the same invertible matrix $A$. The inverse $A^{-1}$ is already known.

**Case 3:** There is one $3\times3$ system for which the inverse matrix is not given. Only one solution vector is needed.

For Cases 2 and 3, describe the method and what can be reused or skipped, without solving an unspecified numerical system completely. Explain the choices using the structure of the matrices and the number of right-hand sides.

## Solution

### Case 1 - Back-substitution

The second equation contains only $y$, so back-substitution is the simplest method. I start with

$$
4y=8
$$

Dividing by $4$ gives $y=2$. I substitute this into the first equation:

$$
2x-2=3
$$

Therefore,

$$
2x=5,\qquad x=\frac52
$$

The solution is

$$
x=\frac52,\qquad y=2
$$

This method uses one division and one substitution. There is no need to calculate an inverse matrix or use full Gaussian elimination because the system is already triangular.

### Case 2 - Use the known inverse

Since the matrix $A$ is invertible and $A^{-1}$ is already known, I would solve each system by multiplying its right-hand side by the inverse:

$$
x_1=A^{-1}b_1
$$

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

The inverse $A^{-1}$ is the same for all three systems. It can be reused for each multiplication, so there is no need to calculate the inverse again or perform a separate elimination for each right-hand side. This choice uses the fact that there are three right-hand sides and the inverse is already available.

### Case 3 - Gaussian elimination

For one $3\times3$ system with an unknown inverse, I would use Gaussian elimination.

First, I would write the augmented matrix from the coefficient matrix and its single right-hand side. Then I would use row operations to make zeros below the pivots and reach row echelon form. Finally, I would use back-substitution to find the three unknowns.

There is only one right-hand side, so I only need to solve one system. Calculating the entire inverse matrix would be extra work that is not necessary for finding this one solution.

## Verification

For Case 1, I substitute the solution into both equations:

$$
2\cdot\frac52-2=5-2=3
$$

$$
4\cdot2=8
$$

Both equations are satisfied.

For Case 2, the proposed method works because, for each right-hand side $b_i$,

$$
A(A^{-1}b_i)=(AA^{-1})b_i=Ib_i=b_i
$$

For Case 3, after elimination and back-substitution, the resulting vector would be checked by multiplying it by the original coefficient matrix to see whether the result equals the given right-hand side. No numerical verification can be performed because Case 3 does not give specific entries of $A$ or $b$.
