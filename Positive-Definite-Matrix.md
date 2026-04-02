# Positive Definite Matrix (正定矩阵)

# Positive Semi-definite Matrix

A positive semi-definite (PSD) matrix/metric is a real symmetric (or **Hermitian**) matrix $`A`$ where the <br>
quadratic form $`x^TAx \ge 0`$ for all vectors $`x`$. **Key characteristics** include **non-negative eigenvalues** <br>
($`\lambda_i \ge 0`$) and the ability to be decomposed as $`A = B^TB`$. Unlike positive definite matrices, PSD <br>
matrices can have a zero determinant and singular values. <sup>Google AI Overview</sup>

## Key Characteristics & Properties

* Definition: For a matrix $`A`$ to be PSD, $`x^TAx \ge 0`$ must hold for all $`x \in R^n`$.
* Eigenvalues: All eigenvalues are real and non-negative ($`\lambda_i \ge 0`$).
* Decomposition: A matrix $`A`$ is PSD if and only if there exists a matrix $`B`$ such that $`A = B^TB`$.
* Diagonal Entries: The diagonal elements $`A_{ii}`$ must be non-negative.
* Sum/Product: The sum of two PSD matrices is PSD, and the **entrywise (Hadamard) product** of two PSD matrices is also PSD.
* Relation to Positive Definite: PSD is a weaker condition than positive definite ($`x^TAx \gt 0`$ and $`\lambda_i \gt 0`$). <br>
  PSD matrices are also referred to as "nonnegative definite".


# Reference
1. [Positive Semi-definite Matrix](http://dsp.ee.cuhk.edu.hk/eleg5481/Lecture%20notes/2-basics/additional/lecture5_linear_algebra.pdf)
2. video: [Positive semi-definite matrices](https://www.youtube.com/watch?v=YofRtrn80gY)
3. video: [Advanced Linear Algebra - Lecture 30: Introduction to Positive (Semi)Definite Matrices](https://www.youtube.com/watch?v=bo8q_HW00wo)
4. [What a Positive (Semi) Definite Matrix Means Visually and Why We Care in ML and Optimization.](https://medium.com/@amehsunday178/what-a-positive-semi-definite-matrix-really-means-and-why-we-care-in-ml-and-optimization-bd427fd12d88) [To Read]
