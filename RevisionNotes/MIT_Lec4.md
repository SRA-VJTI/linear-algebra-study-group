## Factorization into A = LU

    Goal of this lecture is to understand Gaussian elimination in terms of matrices. 
    To ﬁnd a matrix L such that A = LU. 
    We start with some useful facts about matrix multiplication.

### Inverse of a product

* The inverse of a matrix product AB is B <sup>− 1</sup>A <sup>− 1</sup> .

### Transpose of a product

We obtain the <i>transpose</i> of a matrix by exchanging its rows and columns. 

In other words, the entry in row <i>i</i> column <i>j</i> of A is the entry in row <i>j</i> column <i>i</i> of A<sup>T</sup> i.e. <b>A<sub>ij</sub> = (A<sup>T</sup>)<sub>ji</sub></b>

* The transpose of a matrix product AB is B<sup>T</sup>A<sup>T</sup>. 

* For any invertible matrix A, the inverse of A<sup>T</sup> is (A<sup>− 1</sup>)<sup>T</sup>.

### A = LU

We’ve seen how to use elimination to convert a suitable matrix A into an upper triangular matrix U. This leads to the factorization A = LU, which is very helpful in understanding the matrix A.

Recall that (when there are no row exchanges) we can describe the elimination of the entries of matrix A in terms of multiplication by a succession of elimination matrices E<sub>ij</sub> , so that A &rarr; E<sub>21</sub>A &rarr; E<sub>31</sub>E<sub>21</sub>A &rarr; · · · &rarr; U. 

In the 2x2 case this looks like:

![2x2 Elimination](Images/2x2_elimination.png)  

We can convert this to a factorization A = LU by “canceling” the matrix E<sub>21</sub> ;
multiply by its inverse to get (E<sub>21</sub>)<sup>-1</sup>E<sub>21</sub>A = (E<sub>21</sub><sup>-1)</sup>U

![2x2 Elimination Inverse i.e. L](Images/2x2_E_inv.png)

The matrix U is upper triangular with pivots on the diagonal. The matrix L is <i>lower triangular</i> and has ones on the diagonal. Sometimes we will also want to factor out a diagonal matrix whose entries are the pivots:

![A = LDU'](Images/a=ldu'.png)

In the three dimensional case, if E<sub>32</sub>E<sub>31</sub>E<sub>21</sub>A = U then A = E<sub>21</sub><sup>-1</sup>E<sub>31</sub><sup>-1</sup>E<sub>32</sub><sup>-1</sup> U =
LU.

For example, suppose E<sub>31</sub> is the identity matrix and E<sub>32</sub> and E<sub>21</sub> are as
shown below:

![3x3 Elimination](Images/3x3_elimination.png)

The 10 in the lower left corner arises because we subtracted twice the ﬁrst row
from the second row, then subtracted ﬁve times the new second row from the
third.

The factorization A = LU is preferable to the statement EA = U because the combination of row subtractions does not have the effect on L that it did on E. Here L = E<sup>−1</sup> = E<sub>21</sub><sup>-1</sup>E<sub>32</sub><sup>-1</sup> :

![3x3 Elimination Inverse i.e. L](Images/3x3_E_inv.png)

Notice the 0 in row three column one of L = E<sup>−1</sup> , where E had a 10. If there are no row exchanges, the multipliers from the elimination matrices are copied directly into L.

### How expensive is elimination?
Some applications require inverting very large matrices This is done using a computer, of course. How hard will the computer have to work? How long will it take?

When using elimination to ﬁnd the factorization A = LU we just saw that we can build L as we go by keeping track of row subtractions. We have to remember L and (the matrix which will become) U; we don’t have to store A or E ij in the computer’s memory.

How many operations does the computer perform during the elimination process for an n × n matrix? A typical operation is to multiply one row and then subtract it from another, which requires on the order of n operations. There are n rows, so the total number of operations used in eliminating entries in the ﬁrst column is about n<sup>2</sup> . The second row and column are shorter; that product costs about ( n − 1 )<sup>2</sup> operations, and so on. The total number of operations needed to factor A into LU is on the order of n<sup>3</sup> :

![Complexity of Elimination Operation](Images/elimination_complexity.png)

While we’re factoring A we’re also operating on b. That costs about n<sup>2</sup> operations, which is hardly worth counting compared to <sup>1</sup>/<sub>3</sub> ( n<sup>3</sup> ) .

### Row exchanges

What if there are row exchanges? In other words, what happens if there’s a zero in a pivot position?

To swap two rows, we multiply on the left by a permutation matrix. For example,

![Permutation Matrix](Images/permutation_matrix.png)

swaps the ﬁrst and second rows of a 3 × 3 matrix. The inverse of any permutation matrix P is P<sup>−1</sup> = P<sup>T</sup> .

There are n! different ways to permute the rows of an n × n matrix (including the permutation that leaves all rows ﬁxed) so there are n! permutation matrices. These matrices form a multiplicative group.