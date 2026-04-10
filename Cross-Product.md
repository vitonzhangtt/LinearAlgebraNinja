# Cross Product <sup>TODO</sup>

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
* $`n`$ is a **unit vector** perpendicular to the plane containing $`a`$ and $`b`$, with direction such that the ordered set ($`a, b, n`$) is **positively oriented**.


## Conversion to matrix multiplication
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

## Reference
1. wiki: [Cross product](https://en.wikipedia.org/wiki/Cross_product)
2. [Cross products, Math 130 Linear Algebra, D Joyce, Fall 2015](https://math.clarku.edu/~ma130/crossproducts.pdf)
