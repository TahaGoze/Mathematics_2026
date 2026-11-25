# Exercise 1 - Vector Operations and Their Meaning

## Question

Given the vectors

$$
u=(2,-1,3),\qquad v=(-1,4,2)
$$

calculate $u+v$, $u-v$, and $3u-2v$.

Then verify that $(u+v)-v=u$ and explain geometrically what adding two vectors means.

## Solution

Vector addition, subtraction, and scalar multiplication are performed coordinate by coordinate.

### 1. Vector addition

I add the corresponding coordinates of $u$ and $v$:

$$
u+v=(2+(-1),\;-1+4,\;3+2)
$$

Therefore,

$$
u+v=(1,3,5)
$$

### 2. Vector subtraction

I subtract each coordinate of $v$ from the corresponding coordinate of $u$:

$$
u-v=(2-(-1),\;-1-4,\;3-2)
$$

Thus,

$$
u-v=(3,-5,1)
$$

### 3. Calculate 3u-2v

First, I multiply each vector by its scalar:

$$
3u=3(2,-1,3)=(6,-3,9)
$$

$$
2v=2(-1,4,2)=(-2,8,4)
$$

Now I subtract the two results:

$$
3u-2v=(6-(-2),\;-3-8,\;9-4)
$$

Therefore,

$$
3u-2v=(8,-11,5)
$$

### 4. Geometric meaning of vector addition

A vector represents a displacement with a direction and a length. To add $u$ and $v$ geometrically, I place the tail of $v$ at the head of $u$, without changing the direction or length of either vector.

The resulting vector $u+v$ goes from the starting point of $u$ to the final head of $v$. This is called the head-to-tail rule. The same result is the diagonal of the parallelogram formed by $u$ and $v$ when both vectors start at the same point.

## Verification

Using $u+v=(1,3,5)$ and $v=(-1,4,2)$:

$$
(u+v)-v=(1,3,5)-(-1,4,2)
$$

Subtracting the coordinates:

$$
(u+v)-v=(1-(-1),\;3-4,\;5-2)
$$

This gives

$$
(u+v)-v=(2,-1,3)=u
$$

The result is exactly the original vector $u$, so the required identity is verified.

As an additional check, vector subtraction reverses addition:

$$
(u-v)+v=(3,-5,1)+(-1,4,2)
$$

$$
(u-v)+v=(2,-1,3)=u
$$

Both checks confirm that the coordinate operations are correct.
