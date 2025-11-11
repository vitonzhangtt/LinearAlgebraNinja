# Linear Combinations


## Scalar multiplication and addition of matrices

If we say that the shape of a matrix is $`m \times n`$, we mean that it has $`m`$ <br>
rows and $`n`$ columns. For instance, the shape of the matrix below is $`3 \times 4`$: <br>

$`\begin{bmatrix}
0 & 4 & -3 & 1\\
3 & -1 & 2 & 0\\
2 & 0 & -1 & 1
\end{bmatrix}`$

We may also think of the **columns** of a matrix as a set of vectors. For instance, <br>
the matrix above may be represented as

$`\begin{bmatrix}
v_{1}, v_{2}, v_{3}, v_{4}
\end{bmatrix}`$

where <br>
$`v_{1}=\begin{pmatrix}
0\\
3\\
2
\end{pmatrix} \hspace{1cm}  v_{2}=\begin{pmatrix}
4\\
-1\\
0
\end{pmatrix} \hspace{1cm} v_{3}=\begin{pmatrix}
-3\\
2\\
-1
\end{pmatrix} \hspace{1cm}  v_{4}=\begin{pmatrix}
1\\
0\\
1
\end{pmatrix}`$

In this way, we see that the matrix $`3 \times 4`$ is equivalent to an ordered set of 4 vectors <br>
in $`{\mathbb{R}}^3`$.

This means that we may define **scalar multiplication** and **matrix addition** operations using <br>
the corresponding column-wise vector operations. For instance

$`c \times \begin{bmatrix}
v_{1}, v_{2}, v_{3}, v_{4}
\end{bmatrix} = \begin{bmatrix}
cv_{1}, cv_{2}, cv_{3}, cv_{4}
\end{bmatrix}`$

$`\begin{bmatrix}
v_{1}, v_{2}, v_{3}, v_{4}
\end{bmatrix} + \begin{bmatrix}
w_{1}, w_{2}, w_{3}, w_{4}
\end{bmatrix} = \begin{bmatrix}
v_{1}+w_{1}, v_{2}+w_{2}, v_{3}+w_{3}, v_{4}+w_{4}
\end{bmatrix}`$

### Linearity of matrix multiplication
Proposition 2.2.3. Linearity of matrix multiplication.  If $`A`$ is a matrix, <br>
$`v`$ and $`w`$ vectors of the appropriate dimensions, and $`c`$ a scalar, then <br>

* $`A0 = 0`$.
* $`A(cv) = cAv`$.
* $`A(v+w) = Av + Aw`$.

## Matrix-vector multiplication and linear combinations

Definition 2.2.2. **Matrix-vector multiplication**.  The product of a matrix $`A`$ <br>
by a vector $`X`$ will be the **linear combination** of the **columns** of using the <br>
components of $`X`$ as weights. More specifically, if

$`A = \begin{bmatrix}
v_{1}, v_{2}, v_{3}, ..., v_{n}
\end{bmatrix}`$

$`x=\begin{pmatrix}
c_{1}\\
c_{2}\\
\cdot\\
\cdot\\
\cdot\\
c_{n}
\end{pmatrix}`$

then <br>
$`Ax = c_{1}v_{1}+c_{2}v_{2}+...+c_{n}v_{n}`$

If $`A`$ is an $`m \times n`$ matrix, then $`x`$ must be an $`n`$-dimensional vector, <br>
and the product will be an $`m`$-dimensional vector.


The solution space to the equation $`Ax = b`$ is the same as the solution space to the <br> 
linear system corresponding to the **augmented matrix** $`[A | b]`$.

Proposition 2.2.4.  If $`A = [v_{1}, v_{2}, ..., v_{n}]`$ and $`x = \begin{pmatrix}
c_{1}\\
c_{2}\\
\cdot\\
\cdot\\
\cdot\\
c_{n}
\end{pmatrix}`$, then the following statements are equivalent.
* The vector $`x`$ satisfies the equation $`Ax = b`$.
* The vector $`Ax`$ is a linear combination of the columns of $`A`$ with weights $`x_{j}`$:
$`x_{1}v_{1} + x_{2}v_{2} + ... + x_{n}v_{n} = b`$.
* The components of $`x`$ form a solution to the **linear system** corresponding to the **augmented matrix**
  $`[v_{1}, v_{2}, ..., v_{n} | b]`$

## Matrix-matrix products

### Matrix-matrix multiplication

Given matrices $`A`$ and $`B`$, we form their product $`AB`$ by first writing $`B`$ <br>
in terms of its columns <br>

$`B = \begin{bmatrix}
v_{1}, v_{2}, v_{3}, ..., v_{p}
\end{bmatrix}`$

and then defining

$`AB = \begin{bmatrix}
Av_{1}, Av_{2}, Av_{3}, ..., Av_{p}
\end{bmatrix}`$.

### Properties of Matrix-matrix Multiplication
If $`A`$, $`B`$, and $`C`$ are matrices such that the following operations are defined, <br>
it follows that

* Associativity:
$`A(BC) = (AB)C`$
* Distributivity:
  $`A(B+C) = AB + BC`$
  $`(A+B)C = AC + BC`$

#### Caution

The following properties hold for **real numbers** but not for matrices. <br>
* Commutativity: It is not generally true that $`AB = BA`$
* Cancellation: It is not generally true that $`AB = AC`$ implies that $`B = C`$.
* Zero divisors: It is not generally true that $`AB = 0`$ implies that either $`A = 0`$
 or $`B = 0`$. 


## Reference
1. [2.2 Matrix multiplication and linear combinations](https://understandinglinearalgebra.org/sec-matrices-lin-combs.html)



