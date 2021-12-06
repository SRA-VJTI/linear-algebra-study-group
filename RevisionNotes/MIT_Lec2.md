## Elimination with Matrices
 - Process of shifting the position of first non-zero element towards right as we go downwards in a matrix.

 - Pre-multiply A with elimination matrix for changing stuff in rows while doing elimination. For example : E1A = U.

 - Post-multiply A with elimination matrix for changing stuff in columns while doing elimination. For example : AE2 = U.

 - Notice the link between matrix elimination and multiplication from above ideas.

### Permutation matrices
 - A single matrix which when multiplied with A would simplify the process of elimination.

 - A permutation matrix P(PA can be factored into LU) has the same rows as the identity(in some order). There is a single "1" in every row and column. The most common permutation matrix is P = I(exchanges nothing). The product of two permutation matrices is another permutation matrix where the rows of I get reordered twice.

 - P inverse is always equal to P transpose.
  
 - P can produce full set of pivots only in non-singular matrices. In singular cases, no P can produce a full set of pivots.
