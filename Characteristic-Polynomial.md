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
$`\Longleftrightarrow`$ $`(A−λ_{0}I_{n})x=0`$ has a nontrivial solution (In other words $`Nul(A−λ_{0}I_{n}) \neq 0`$. [Nul(A)](https://github.com/vitonzhangtt/LinearAlgebraNinja/blob/main/Subspace.md#null-space-2)) <br>
$`\Longleftrightarrow`$ $`A−λ_{0}I_{n}`$ is not invertible <br>
$`\Longleftrightarrow`$ $`det(A−λ_{0}I_{n})=0`$ <br>
$`\Longleftrightarrow`$ $`f(λ_{0})=0`$.

#### Nontrivial Solution in Linear Algebra <sup>Google AI Overview</sup>

A **nontrivial solution**(非平凡解) in linear algebra is any solution to a homogeneous system of <br>
linear equations ($`Ax=0`$) where at least one variable in the solution vector $`x`$ <br>
is **non-zero**. While the **trivial solution** ($`x=0`$) always satisfies $`Ax=0`$, <br>
a nontrivial solution exists if and only if the matrix $`A`$ is **not invertible**, <br>
the **rank** of $`A`$ is less than the number of variables, or there is at least one <br>
free variable. 


## Determinant and Eigenvalues <sup>Google AI Overview</sup>

The determinant of a **square** matrix $`A`$ of **order** $`n`$ is exactly equal to the product <br>
of its $`n`$ eigenvalues.

$`\det (A)=\prod _{i=1}^{n}\lambda _{i}=\lambda _{1}\lambda _{2}\dots \lambda _{n}`$

### Key Concepts 

* Algebraic Multiplicity: When calculating this product, each eigenvalue must be included as many <br>
  times as its multiplicity.
* Characteristic Polynomial Connection: The **characteristic polynomial** of a matrix $`A`$ is defined <br>
  as $`p(\lambda )=\det (A-\lambda I)`$. Setting $`\lambda =0`$ in this polynomial yields $`\det (A)`$, 
  which also corresponds to <br> the constant term of the polynomial formed by the product of its roots (the **eigenvalues**).
* Trace Relationship: While the product of eigenvalues is the determinant, their sum is equal to the trace <br>
   of the matrix (the sum of the diagonal elements).
* Invertibility: A matrix is invertible if and only if its determinant is non-zero, which implies that <br>
  none of its eigenvalues can be zero.
* Geometric Intuition: The **absolute value of the determinant** represents the factor by which the <br>
  matrix scales the volume of a region in space. In a basis of eigenvectors (for diagonalizable matrices), <br>
  this is simply the product of the scaling factors along each eigenvector's axis. 

### Step-by-step Proof

The standard proof that the determinant of a matrix $`A`$ equals the product of its eigenvalues 
involves analyzing the **characteristic polynomial**, $`p(\lambda )=\det (A-\lambda I)`$. 

* Define the Characteristic Polynomial: For an $`n\times n`$ matrix $`A`$, the characteristic <br>
  polynomial is given by: <br>
  $`p(\lambda )=\det (A-\lambda I)`$ <br>
  The roots of this polynomial are the eigenvalues ($`\lambda _{1},\lambda _{2},\dots ,\lambda _{n}`$) of the matrix $`A`$.
* Factor the Polynomial: According to the **Fundamental Theorem of Algebra** [FTA](https://github.com/vitonzhangtt/MathNinja/blob/main/Fundamental-Theorem-of-Algebra.md), any <br>
  polynomial of degree $`n`$ can be factored into $`n`$ linear factors using **its roots**: <br>
  $`p(\lambda )=(c)(\lambda _{1}-\lambda )(\lambda _{2}-\lambda )\dots (\lambda _{n}-\lambda )`$ <br>
  In the specific expansion of $`\det (A-\lambda I)`$, the leading coefficient $`c`$ is always 1 <br>
  (if defined as $`|\lambda I-A|`$) or depends on $`(-1)^{n}`$ (if defined as $`|A-\lambda I|`$). <br>
  Let's use the form:$`p(\lambda )=(\lambda _{1}-\lambda )(\lambda _{2}-\lambda )\dots (\lambda _{n}-\lambda )`$
* Evaluate at $`\lambda =0`$: To find the relationship between the determinant and the eigenvalues, <br>
  we evaluate the polynomial at $`\lambda =0`$:
  * From the definition: $`p(0)=\det (A-0\cdot I)=\det (A)`$.
  * From the factored form: $`p(0)=(\lambda _{1}-0)(\lambda _{2}-0)\dots (\lambda _{n}-0)=\lambda _{1}\lambda _{2}\dots \lambda _{n}`$.
* Conclusion: Since both expressions equal $`p(0)`$, we conclude:$`\det (A)=\prod _{i=1}^{n}\lambda _{i}`$ <br>
  This result holds for all **square matrices**, including those with repeated eigenvalues (multiplicity) and <br>
  those that are not diagonalizable.

### Intuitive "Diagonal" Case 

If a matrix is **diagonalizable**, the proof is even simpler. Such a matrix can be written <br>
as $`A=PDP^{-1}`$, where $`D`$ is a **diagonal matrix** containing the eigenvalues. <br>
Using the property that **the determinant of a product is the product of the determinants**: <br>
$`\det (A)=\det (P)\det (D)\det (P^{-1})`$ <br>
Since $`\det (P^{-1})=1/\det (P)`$, these terms <br>
cancel out, leaving:$`\det (A)=\det (D)=\lambda _{1}\lambda _{2}\dots \lambda _{n}`$


## Properties of the Characteristic Polynomial
TODO: [1]

# Reference
1. [Characteristic Equation: Everything You Need to Know for Data Science](https://www.datacamp.com/tutorial/characteristic-equation) [To Read]
2. [5.2The Characteristic Polynomial](https://textbooks.math.gatech.edu/ila/characteristic-polynomial.html) from `Interactive Linear Algebra`
