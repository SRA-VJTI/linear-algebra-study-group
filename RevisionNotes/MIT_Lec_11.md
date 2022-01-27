# 11 - Bases of new vector spaces, Rank one matrices

**All for 3x3 cases**
* Basis - 9 dimensional (1 at each cell)
* Basis of symmetric matrices - 6 dimensional
* Basis of upper triangular matrices - 6 dimensional
* Basis of (Symmetric ∩ Upper triangular) - 3 dimensional (since diagonal)
* Basis of (Symmetric ∪ Upper triangular) - 9 dimensional (since all 3x3)
* dim(S) + dim(U) = dim(S ∩ U) + dim(S ∪ U), where S and U are vector spaces.

* Every rank 1 matrix can be expressed as - u x v<sup>T</sup>
  * where `u` and `v` are column matrices

* Let M be all 5x17 matrices with rank 4. Is M a subspace?
  * No. Since no `0` matrix

**Some extra conditions for a double sided inverse**
* The rows of A span R<sup>n</sup>.
* The rows are linearly independent.
* Elimination can be completed: PA = LDU, with all n pivots.
* Zero is not an eigenvalue of A.
* A<sup>T</sup>A is positive definite.
