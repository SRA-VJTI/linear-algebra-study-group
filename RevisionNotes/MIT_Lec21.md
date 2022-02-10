# Eigenvalues and Eigenvectors

A matrix A acts on vectors x like a function does, with input x and output Ax.

Eigenvectors are vectors for which Ax is parallel to x. In other words:

    Ax = λx.

In this equation, x is an eigenvector of A and λ is an eigenvalue of A.

If the eigenvalue λ equals 0 then Ax = 0x = 0. Vectors with eigenvalue 0 make
up the nullspace of A; if A is singular, then λ = 0 is an eigenvalue of A.

## det ( A − λI ) = 0

* In order to get a non-zero eigenvector, A − λI must be singular. In other words,
det ( A − λI ) = 0. We can solve this characteristic equation for λ to get n solutions.

* An (**n x n**) matrix will have **n** eigenvalues, and their sum will be the sum of the diagonal entries of the matrix: a<sub>11</sub> + a<sub>22</sub> + · · · + a<sub>nn</sub> . This sum is the trace of the matrix. For a two by two matrix, if we know one eigenvalue we can use this fact to ﬁnd the second.

* We might get n distinct eigenvalues or 1 or more repeated eigenvalues. 

* In general, the eigenvalues of a two by two matrix are the solutions to:

    λ<sup>2</sup> − trace ( A ) · λ + det A = 0

* Once we’ve found an eigenvalue λ, we can use elimination to ﬁnd the nullspace of A − λI. The vectors in that nullspace are eigenvectors of A with eigenvalue λ.



## Examples

* Suppose P is the matrix of a projection onto a plane. For any **x** in the plane
P**x** = **x**, so **x** is an eigenvector with eigenvalue 1. 

* A vector **x** perpendicular to the plane has P**x** = 0, so this is an eigenvector with eigenvalue λ = 0. The eigenvectors of P span the whole space (but this is not true for every matrix).

* Real eigenvalues

    ![Example](Images/eigen_eg1_lec21.png)

    <details>
    <summary>Eigenvalues</summary>
    1, -1
    </details>

    <details>
    <summary>Eigenvectors</summary>
    [1,1] with λ = 1, [1,-1] with λ = -1
    </details>

    ![Example](Images/eigen_eg2_lec21.png)

    <details>
    <summary>Eigenvalues</summary>
    4, 2
    </details>

    <details>
    <summary>Eigenvectors</summary>
    [1,1] with λ = 1, [1,-1] with λ = -1
    </details>

    **Note**: 
    * The eigenvectors of A are the same as those of B. Adding 3I to the matrix B added 3 to each of its eigenvalues and did not change its eigenvectors, because Ax = ( B + 3I ) x = λx + 3x = ( λ + 3 ) x.
    * The eigenvalues of the sum (A+B) and product AB aren’t usually equal to the sum λ ( A ) + λ ( b ) and product λ ( A ) λ ( b ) respectively.

* Complex eigenvalues

    ![Example](Images/eigen_complex_lec21.png)

    <details>
    <summary>Eigenvalues</summary>
    i, -i
    </details>

    **Note**:
    * If a matrix has a complex eigenvalue a + bi then the complex conjugate a − bi is also an eigenvalue of that matrix.
    * Symmetric matrices have real eigenvalues. For antisymmetric matrices like Q, for which A<sup>T</sup> = − A, all eigenvalues are imaginary (λ = bi).

* Triangular matrices and repeated eigenvalues

    ![Example](Images/eigen_repeat_lec21.png)

    <details>
    <summary>Eigenvalues</summary>
    3, 3
    </details>
    <details>
    <summary>Eigenvectors</summary>
    [1,0]
    </details>