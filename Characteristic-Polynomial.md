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

Theorem(Eigenvalues are roots of the characteristic polynomial) Let $`A`$ be an $`n×n`$ matrix, and let <br> 
$`f(λ)=det(A−λI_{n})`$ be its characteristic polynomial. Then a number $`λ_{0}`$ is an eigenvalue of $`A`$ if and only if <br>
$`f(λ_{0})=0`$.




## Properties of the Characteristic Polynomial


# Reference
1. [Characteristic Equation: Everything You Need to Know for Data Science](https://www.datacamp.com/tutorial/characteristic-equation)
2. [5.2The Characteristic Polynomial](https://textbooks.math.gatech.edu/ila/characteristic-polynomial.html) from `Interactive Linear Algebra`
