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

## Matrix-vector multiplication and linear combinations

Definition 2.2.2. **Matrix-vector multiplication**.  The product of a matrix $`A`$ 
by a vector $`X`$ will be the **linear combination** of the columns of using the 
components of $`X`$ as weights. More specifically, if





## Reference
1. [2.2 Matrix multiplication and linear combinations](https://understandinglinearalgebra.org/sec-matrices-lin-combs.html)



