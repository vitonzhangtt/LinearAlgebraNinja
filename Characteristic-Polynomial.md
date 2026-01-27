# Characteristic Polynomial (特征多项式)

## Definition <sup>[2]</sup>

Let $`A`$ be an $`n×n`$ matrix. The **characteristic polynomial** of $`A`$ is the function $`f(λ)`$ given by

$`f(\lambda) = det(A-\lambda I_{n})`$

Finding the characterestic polynomial means computing the determinant of the matrix <br>
$`A−λI_{n}`$, whose entries contain the unknown $`λ`$.

**The point of the characteristic polynomial** is that we can use it to compute eigenvalues.

### Examples

<img width="760" height="400" alt="from [2]" src="https://github.com/user-attachments/assets/ff0ebe4c-c944-439a-8dcb-91a869f0a4d6" />

## Eigenvalues are roots of the characteristic polynomial <sup>[2]</sup>

Theorem (Eigenvalues are roots of the characteristic polynomial): Let $`A`$ be an $`n×n`$ matrix, and let <br> 
$`f(λ)=det(A−λI_{n})`$ be its characteristic polynomial. Then a number $`λ_{0}`$ is an eigenvalue of $`A`$ if and only if <br>
$`f(λ_{0})=0`$.

### Proof

By the [Invertible Matrix Theorem](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Invertible-Matrix.md#invertible-matrix-theorem-1), the matrix equation $`(A−λ_{0}I_{n})x=0`$ <br>
has a **nontrivial solution** if and only if $`det(A−λ_{0}I_{n})=0`$.
Therefore, 
 
$`λ_{0}`$ is an eigenvalue of A <br>
$`\Longleftrightarrow`$ $`Ax=λ_{0}x`$ has a nontrivial solution <br>
$`\Longleftrightarrow`$ $`(A−λ_{0}I_{n})x=0`$ has a nontrivial solution (In other words $`Nul(A−λ_{0}I_{n}) \neq 0`$) <br>
$`\Longleftrightarrow`$ $`A−λ_{0}I_{n}`$ is not invertible <br>
$`\Longleftrightarrow`$ $`det(A−λ_{0}I_{n})=0`$ <br>
$`\Longleftrightarrow`$ $`f(λ_{0})=0`$.

#### Nontrivial Solution in Linear Algebra <sup>Google AI Overview</sup>

A **nontrivial solution** in linear algebra is any solution to a homogeneous system of <br>
linear equations ($`Ax=0`$) where at least one variable in the solution vector $`x`$ <br>
is **non-zero**. While the trivial solution ($`x=0`$) always satisfies $`Ax=0`$, <br>
a nontrivial solution exists if and only if the matrix $`A`$ is **not invertible**, <br>
the **rank** of $`A`$ is less than the number of variables, or there is at least one <br>
free variable. 


## Properties of the Characteristic Polynomial


# Reference
1. [Characteristic Equation: Everything You Need to Know for Data Science](https://www.datacamp.com/tutorial/characteristic-equation)
2. [5.2The Characteristic Polynomial](https://textbooks.math.gatech.edu/ila/characteristic-polynomial.html) from `Interactive Linear Algebra`
