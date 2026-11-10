
# Exercise 14 - Rotation Matrices

## Question

R(t) = [[cos(t), -sin(t)], [sin(t), cos(t)]]

Show that R(alpha)R(beta) = R(alpha + beta).

Explain the result geometrically.

## Solution

First, multiply the two matrices:

R(alpha)R(beta) =

[[cos(alpha)cos(beta) - sin(alpha)sin(beta),
  -cos(alpha)sin(beta) - sin(alpha)cos(beta)],

 [sin(alpha)cos(beta) + cos(alpha)sin(beta),
  -sin(alpha)sin(beta) + cos(alpha)cos(beta)]]

Now use the angle-sum formulas:

cos(alpha + beta) =
cos(alpha)cos(beta) - sin(alpha)sin(beta)

sin(alpha + beta) =
sin(alpha)cos(beta) + cos(alpha)sin(beta)

So the result becomes:

[[cos(alpha + beta), -sin(alpha + beta)],
 [sin(alpha + beta), cos(alpha + beta)]]

This is exactly R(alpha + beta).

Therefore:

R(alpha)R(beta) = R(alpha + beta)

## Verification and Explanation

Rotating by beta and then by alpha gives a total rotation of alpha + beta.

For example, rotating 90 degrees two times gives a total rotation of 180 degrees.

This agrees with the matrix formula.
