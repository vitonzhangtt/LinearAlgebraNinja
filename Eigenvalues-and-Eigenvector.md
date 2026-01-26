# Eigenvalues and Eigenvector (特征值和特征向量)

## Definition
Definition 4.1.1.  Given a square $`n \times n`$ matrix $`A`$, we say that a nonzero vector $`v`$ <br>
is an eigenvector of $`A`$ if there is a scalar $`\lambda`$ such that

$`Av = \lambda v`$.

The scalar $`\lambda`$ is called the **eigenvalue** associated to the **eigenvector** $`v`$.

## Eigen Value Decomposition (EVD) 

Eigenvalue decomposition (EVD) is a matrix factorization method in linear algebra that breaks <br>
down a **diagonalizable** square matrix $`A`$ into its constituents: **eigenvectors** and **eigenvalues**. <br>
Expressed as $`A=V\Lambda V^{-1}`$, it separates a linear transformation into scaling <br>
(diagonal matrix $`\Lambda`$) and direction (eigenvector matrix $`V`$), simplifying matrix powers <br>
and applications like PCA. <sup>Google AI Overview</sup>

### Key Components and Concepts <sup>Google AI Overview</sup>

* Definition: For a square matrix $`A`$, a scalar $`\lambda`$ (eigenvalue) and a non-zero vector <br>
  $`v`$ (eigenvector) satisfy $`Av=\lambda v`$.
* Formula: $`A=V\Lambda V^{-1}`$, where $`V`$ is a matrix with **eigenvectors as columns**, and $`\Lambda`$ <br>
  is a diagonal matrix containing corresponding eigenvalues.
* Diagonalization: Only diagonalizable matrices can be decomposed this way.
* Spectral Decomposition: For real symmetric matrices, the decomposition is $`A=Q\Lambda Q^{T}`$, <br>
  where $`Q`$ is an orthogonal matrix ($`Q^{-1}=Q^{T}`$). 

### Steps to Compute Eigendecomposition <sup>Google AI Overview</sup>

* Find Eigenvalues ($`\lambda `$): Solve the characteristic equation $`\det (A-\lambda I)=0`$, <br>
where $`I`$ is the identity matrix.
* Find Eigenvectors ($`v`$): For each $`\lambda `$, solve the linear system $`(A-\lambda I)v=0`$.
* Construct Matrices: Form $`\Lambda `$ from eigenvalues and $`V`$ from corresponding eigenvectors. 

### Applications <sup>Google AI Overview</sup>

* Principal Component Analysis (PCA): Reducing dimensionality in data analysis.
* Matrix Powers: Calculating $`A^{k}=V\Lambda ^{k}V^{-1}`$ efficiently.
* System Stability: Analyzing dynamic systems in engineering and physics.
* Google PageRank: Determining the importance of web pages. 


## Applications


## Reference
1. [4.1 An introduction to eigenvalues and eigenvectors](https://understandinglinearalgebra.org/sec-eigen-intro.html)
2. [Linear Algebra for AI: Part 7 — Eigen Decomposition](https://medium.com/@ebimsv/mastering-linear-algebra-part-7-eigen-decomposition-cf3c50308ba7)
3. [Linear Algebra for AI: Part 1 — Introduction to Linear Algebra in Machine Learning](https://medium.com/@ebimsv/mastering-linear-algebra-part-1-introduction-to-linear-algebra-in-machine-learning-fafcae1a5879) (AAAA) [To Read]
4. [Eigendecomposition: A Beginner's Guide to Matrix Factorization](https://www.datacamp.com/tutorial/eigendecomposition)
