# Autocorrelation Matrix

An autocorrelation matrix is a **square, symmetric**, and usually **Toeplitz** matrix <br>
representing the correlations between **different time points** of a **stochastic process** <br>
or random vector ($`E[X_{i}X_{j}]`$). It is fundamental in signal processing, <br>
linear prediction, and system identification, often used for spectral analysis, <br>
determining energy concentration, and solving efficient linear equations via <br>
**Levinson-Durbin** recursion. <sup>Google AI Overview</sup>

The autocorrelation matrix is a fundamental construct in signal processing and related fields, <br>
defined as a matrix representing the **autocorrelation function** of a signal. <sup>[1]</sup>

## Autocorrelation Function

## Mathematical Foundations and Properties <sup>[1]</sup>

The (potentially time-dependent) autocorrelation matrix (also called **second moment**) of <br>
a (potentially time-dependent) random vector $` \mathbf {X} =(X_{1},\ldots ,X_{n})^{\rm {T}}`$ is <br>
an $`{\displaystyle n\times n}`$ matrix containing as elements the autocorrelations of all pairs <br>
of elements of the random vector $`{\displaystyle \mathbf {X} }`$. The autocorrelation matrix is <br>
used in various digital signal processing algorithms.

For a random vector $`{\displaystyle \mathbf {X} =(X_{1},\ldots ,X_{n})^{\rm {T}}}`$ containing random <br>
elements whose expected value and variance exist, the autocorrelation matrix is defined by

$`{\displaystyle {R} _{\mathbf {X} \mathbf {X} }\triangleq \  {E} \left[\mathbf {X} \mathbf {X} ^{\rm {T}}\right]}`$

where $`{\displaystyle {}^{\rm {T}}}`$ denotes the transposed matrix of dimensions $`{\displaystyle n\times n}`$.

Written component-wise:

$`{\displaystyle {R} _{\mathbf {X} \mathbf {X} }={
  \begin{bmatrix} 
    {E} [X_{1}X_{1}]& {E} [X_{1}X_{2}]&\cdots & {E} [X_{1}X_{n}]  \\
    {E} [X_{2}X_{1}]& {E} [X_{2}X_{2}]&\cdots & {E} [X_{2}X_{n}]  \\
    \vdots &\vdots &\ddots &\vdots \\
    {E} [X_{n}X_{1}]& {E} [X_{n}X_{2}]&\cdots & {E} [X_{n}X_{n}]
  \end{bmatrix}
  }
  }`$


## Uncertainty Ellipse (or Covariance Ellipse) <sup>Google AI Overview</sup>

**Uncertainty ellipse** (or **covariance ellipse**) analysis uses the **eigenvalues** and **eigenvectors** <br>
of an autocorrelation (or covariance) matrix to **geometrically** characterize the uncertainty in <br>
2D or 3D data. The **eigenvalues** represent the **variance of the data** along the **principal axes** <br>
(magnitudes), while the **eigenvectors** represent the **orientation of these axes**. 

### Core Concepts 

* Autocorrelation/Covariance Matrix: A **symmetric**, **positive semi-definite** matrix that encapsulates <br>
  the variances of variables and the **covariances** between them.
* Eigenvalues ($`\lambda _{i}`$): The eigenvalues of the covariance matrix represent the amount of <br>
  variance (spread) along the corresponding eigenvectors (principal components).
* Eigenvectors ($`v_{i}`$): These define the orthogonal directions of the ellipse's axes.
* The Ellipse: An ellipse represents **a contour of equal probability density for a bivariate normal** <br>
  **distribution**. Its shape (flattening) depends on the **correlation strength**, varying from a circle <br>
  (uncorrelated) to a line (perfectly correlated).

### Eigenvalue Analysis for Error Ellipses 

For a $`2\times 2`$ covariance matrix, the eigenvalues $`\lambda _{1}`$ and $`\lambda _{2}`$ (where <br>
$`\lambda _{1}\ge \lambda _{2}`$) determine the size of the ellipse axes: 

1. Major Axis Length: Proportional to $`\sqrt{\lambda _{1}}`$.
2. Minor Axis Length: Proportional to $`\sqrt{\lambda _{2}}`$.
3. Orientation: The angle of the major axis is determined by the eigenvector corresponding to $`\lambda _{1}`$. 

#### Key Findings

* Uncorrelated Data: If the variables are uncorrelated, the **covariance matrix** is **diagonal**, <br>
  the eigenvectors align with the coordinate axes, and the ellipse axes are parallel to <br>
  the $`x`$ and $`y`$ axes.
* Correlated Data: If the correlation is non-zero, the ellipse is rotated and stretched along <br>
  a diagonal direction.
* Confidence Levels: The 95% confidence ellipse is typically used to represent the uncertainty, <br>
  usually drawn with axes scaled by a factor (e.g., $`\sqrt{F_{2,n}(0.95)}`$). 

### Applications 
* Position Error Analysis: In surveying and navigation, it defines the probable area where a <br>
  point lies, given **covariance matrix** elements ($`\sigma _{x},\sigma _{y},\sigma _{xy}`$).
* Principal Component Analysis (PCA): **Eigendecomposition** of a covariance matrix is used to find <br>
  the directions of maximum variance.
* Signal Processing: Eigenvalues of an autocorrelation matrix help identify hidden periodicities <br>
   or signal characteristics.
* Feature Detection: The **eigenvalue spread** (ratio of maximum to minimum eigenvalues) is used to <br>
  detect corner points in images, where a **high spread indicates edge-like**, rather than <br>
  corner-like, structures. 


# Reference
1. wiki: [Autocorrelation of random vectors](https://en.wikipedia.org/wiki/Autocorrelation#Autocorrelation_of_random_vectors)
