# Cross Product

## Definition

The cross product of two vectors $`a`$ and $`b`$ is defined only in <br> 
three-dimensional space and is denoted by $`a × b`$. <sup>[1]</sup>

The cross product $`× : R^{3} × R^{3} → R^{3} `$ is an operation that takes two vectors $`u`$ and <br>
$`v`$ in space and determines another vector $`u×v`$ in space. <sup>[2]</sup>

The cross product $`a \times b`$ is defined as a vector $`c`$ that is **perpendicular** (orthogonal) to both $`a`$ 
and $`b`$, with a direction given by the **right-hand rule** and a magnitude equal to the area of the parallelogram
that the vectors span. <sup>[1]</sup>

The cross product is defined by the formula: <sup>[1]</sup>

$`\mathbf {a} \times \mathbf {b} =\left\|\mathbf {a} \right\|\left\|\mathbf {b} \right\|\sin(\theta )\,\mathbf {n}`$ ,

where

* $`θ`$ is the angle between $`a`$ and $`b`$ in the plane containing them (hence, it is between 0° and 180°),
* $`‖a‖`$ and $`‖b‖`$ are the magnitudes of vectors $`a`$ and $`b`$,
* $`n`$ is a **unit vector** **perpendicular** to the plane containing $`a`$ and $`b`$, with direction such that the ordered set ($`a, b, n`$) is **positively oriented**.

### 3D Space

In three-dimensional space, the **cross product** is defined as the **determinant** of a $`3 \times 3`$ matrix where:

* The first row consists of the unit vectors $`i,j,k`$.
* The second row consists of the components of the first vector, $`a=(a_1, a_2, a_3)`$.
* The third row consists of the components of the second vector, $`b=(b_1, b_2, b_3)`$.

The Formula:

<img width="194" height="76" alt="" src="https://github.com/user-attachments/assets/9e8138c9-ff96-4f25-936b-a69b51efcfd6" />

To solve this, you expand along the top row:

<img width="480" height="32" alt="" src="https://github.com/user-attachments/assets/b566b9ff-7c6e-4a67-af12-6d1303973091" />




## Conversion to matrix multiplication

The cross product of two vectors, $`a \times b`$, can be represented as the multiplication of a **skew-symmetric matrix**
$`[a]_{\times}`$ and the vector $`b`$. This matrix representation transforms the vector operation into linear matrix algebra: $`a \times b = [a]_{\times} b`$. (**NOTE**: Sometimes we also write $`[a]_{\times}`$ as $`[a]`$)

### Proof

How to prove $`a \times b = [a]_{\times} b`$?


### Example
Let $`\vec{a} = {(a_{1}, a_{2}, a_{3})}`$ and $`\vec{b} = {(b_{1}, b_{2}, b_{3})}`$, then
$`\vec{a} \times \vec{b} = [\vec{a}]{\vec{b}}`$. The $`[\vec{a}]`$ is defined as the following <br>

$`
[\vec{a}] = 
  \begin{bmatrix}
    0 & -a_{3} & a_{2}    \\
    a_{3} & 0 & -a_{1}    \\
    -a_{2} & a_{1} & 0    \\
  \end{bmatrix}
`$

## Properties of the Cross Product

* **Vector Nature**: The result is a **pseudovector** that is orthogonal (perpendicular) to the plane <br>
  containing both vectors.
* **Direction** (**Right-Hand Rule**): If you curl the fingers of your right hand from $`a`$ to $`b`$, your <br>
  thumb points in the direction of $`a \times b`$.
* **Anti-commutative**: Reversing the order of vectors negates the result: $`a \times b = -(b \times a)`$.
* **Distributive**: The cross product distributes over addition: $`a \times (b+c) = a \times b + a \times c`$.
* **Zero Vector**: The cross product of two parallel or antiparallel vectors is zero ($`a \times a = 0`$).
* **Scalar Multiplication**: Compatible with scalars ($`c`$ is a scalar): $`(ca) \times b = a \times (cb) = c (a \times b)`$.
* **Magnitude and Area**: The magnitude $`|a \times b|`$ is the area of the **parallelogram** formed by the vectors, <br>
  and $`\frac{1}{2}|a \times b|`$ is the area of the triangle formed by them.
* **Unit Vector Cross Products**: Following the Right-Hand Rule: $`i \times j = k`$, $`j \times k = i`$, and $`k \times i = j`$.
* **Not Associative**: $`a \times (b \times c)`$ is not generally equal to $`(a \times b) \times c`$.
* **Not Commutative**: $`a \times b \neq b \times a`$ (unless the product is zero).

## Identities

### Identity: $`a \cdot (b \times c) = (a \times b) \cdot c`$

The easiest way to see this is through the [**determinant definition**](). Both sides of the equation represent <br>
the **volume** of a **parallelepiped**(平行六面体) formed by the three vectors.

* Left Side: $`a \cdot (b \times c)`$ is the determinant of a $`3 \times 3`$ matrix with rows $`a, b, c`$:

<img width="230" height="71" alt="" src="https://github.com/user-attachments/assets/b360a6ae-f46e-42a6-92b2-46138dbac894" />






## Reference
1. wiki: [Cross product](https://en.wikipedia.org/wiki/Cross_product)
2. [Cross products, Math 130 Linear Algebra, D Joyce, Fall 2015](https://math.clarku.edu/~ma130/crossproducts.pdf)
