# Determinant

TODO

## Defintion as Cross Product in 3D



## Row Swapping Property

The row swapping property (often called the **sign property** or **switching property**) states that if you <br>
interchange any two rows (or any two columns) of a **square matrix**, the **sign** of its determinant flips. <br>
If the original determinant is $`D`$, after one swap, the new determinant is $`-D`$.

* Single Swap: Multiplies the determinant by $`-1`$.
* Multiple Swaps: If you perform $`n`$ swaps, the determinant is multiplied by $`(-1)^n`$.
  * An even number of swaps keeps the same sign.
  * An odd number of swaps changes the sign.
* Zero Determinant: If a determinant is $`0`$, swapping rows leaves it at $`0`$ (since $`-0 = 0`$).

### Why This Happens

Geometrically, the determinant represents the **signed volume of a shape**. Swapping two rows is equivalent <br> 
to a reflection in space, which flips the orientation (e.g., from a right-handed system to a left-handed system), <br> 
causing the sign change.


# Reference
1. [4.1 Determinants: Definition](https://textbooks.math.gatech.edu/ila/determinants-definitions-properties.html) from `Interactive Linear Algebra`
2. [The Determinant: How It Works and What It Tells Us](https://www.datacamp.com/tutorial/determinant)
