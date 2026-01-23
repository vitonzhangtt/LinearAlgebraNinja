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

# Reference
1. wiki: [Autocorrelation of random vectors](https://en.wikipedia.org/wiki/Autocorrelation#Autocorrelation_of_random_vectors)
