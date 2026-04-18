# Inner Product


# Inner Product Space

## Google AI Overview

An inner product space is a **vector space** (real or complex) paired with a **function**—the **inner product**—that <br>
assigns **a scalar** to each pair of vectors, enabling the calculation of vector **lengths, angles, and orthogonality**. <br>
It **generalizes** the **Euclidean dot product**, defined by **linearity**, **symmetry** (conjugate symmetry for complex <br>
spaces), and **positive-definiteness** ($`\langle v, v \rangle \ge 0`$).

### Key Properties

* Linearity: $`\langle au+bv, w \rangle = a\langle u + w \rangle+b\langle v+w \rangle`$
* Symmetry/Hermitian: $`\langle v, u \rangle = \overline{\langle v, u \rangle}`$ (for real spaces,
  $`\langle v, u \rangle = \langle u, v \rangle`$).
* Positive Definiteness: $`\langle v, v \rangle \ge 0`$, and $`\langle v, v \rangle = 0`$ if and only if $`v = 0`$.
* Induced Norm (Length): $`\Vert v \Vert = \sqrt{\langle v, v \rangle}`$.
* Distance: $`d(u, v) = \Vert u-v \Vert = \sqrt{\langle u-v, u-v \rangle}`$












Inner product spaces are foundational in **functional analysis** (specifically **Hilbert spaces**) for defining <br>
orthogonality, allowing for projections and Fourier series analysis.

## vs. Hilbert Spaces

# Dot Product

## Geometric Interpretation

The **dot product** of two vectors $`a`$ and $`b`$ measures how much they align, calculated as $`a \cdot b = \lVert a \rVert \lVert b \rVert cos(\theta)`$. <br>
It represents the **projection** of one vector onto another, multiplied by the magnitude of the second vector. <br>
The result indicates **direction similarity**: **positive (same direction)**, **zero (perpendicular)**, or <br>
**negative (opposite directions)**.

### Key Geometric Interpretations

* Projection Method: The dot product $`a \cdot b`$ is the length of the projection of vector $`a`$ onto vector <br>
  $`b`$ (i.e., $`\lVert a \rVert cos(\theta)`$), scaled by the length of $`b`$ ($`\lVert b \rVert`$).
* Alignment Indicator: The sign of the dot product shows how similar the directions are:
  * Positive: Vectors point in generally the same direction ($`\theta \lt 90^{\circ}`$).
  * Zero: Vectors are perpendicular ($`90^{\circ}`$ or **orthogonal**), indicating no projection.
  * Negative: Vectors point in generally opposite directions ($`\theta \gt 90^{\circ}`$).
* Component Representation: If $`a`$ is a unit vector (length $`1`$), $`a \cdot b`$ directly gives the magnitude of 
  the projection of $`b`$ onto $`a`$.

### Commutative Property

The dot product (or scalar product) satisfies the commutative property. 

For any two real vectors $`a`$ and $`b`$, the order of the operation does not change the result: $`a \cdot b = b \cdot a`$.



# Reference
1. [6.1 Inner Products](https://dusolution.wordpress.com/wp-content/uploads/2015/06/elementary_linear_algebra_10th_edition.pdf) from Book: `Elementary Linear Algebra 10th 2010` 
