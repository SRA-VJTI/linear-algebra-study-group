# Applications of Determinants
We know a formula for and some properties of the determinant. Now we see
how the determinant can be used.
## Formula for A<sup>-1</sup>

<b>A<sup>-1</sup> = C<sup>T</sup>/det(A)</b>


To verify the formula, we’ll check that AC<sup>T</sup> = (det A) I.

![Verifying A-1 formula](Images/ACt_lec20.png)

The entry in the ﬁrst row and ﬁrst column of the product matrix is:

![Verifying A-1 formula](Images/ACt_11_lec20.png)

(This is just the cofactor formula for the determinant.) This happens for every
entry on the diagonal of AC<sup>T</sup> .

To ﬁnish proving that AC<sup>T</sup> = (det A) I, we just need to check that the off-
diagonal entries of AC<sup>T</sup> are zero. In the two by two case, multiplying the en­
tries in row 1 of A by the entries
in column
2 of C<sup>T</sup> gives a (− b ) + b ( a ) = 0.

This is the determinant of A<sub>s</sub>:

![Verifying A-1 formula](Images/As_lec20.png)

In higher dimensions, the product of the ﬁrst row of A and the last column of C<sup>T</sup> equals the determinant of a matrix
whose ﬁrst and last rows are identical. This happens with all the off diagonal
matrices, which conﬁrms that A<sup>−1</sup> = C<sup>T</sup>/(detA)

## Cramer’s Rule for x = A<sup>−1</sup>b
We know that if Ax = b and A is nonsingular, then x = A<sup>−1</sup>b. Applying the formula A<sup>−1</sup> = C<sup>T</sup>/(detA) gives us:

**x = C<sup>T</sup>b/(detA)**

Cramer’s rule gives us another way of looking at this equation. To derive
this rule we break x down into its components. Because the i’th component of C<sup>T</sup> b is a sum of cofactors times some number, it is the determinant of some matrix B<sub>j<sub>.

**x<sub>j</sub> = det(B<sub>j</sub>)/det(A)**

where B<sub>j</sub> is the matrix created by starting with A and then replacing column j with b, so:

![Verifying Cramer's rule](Images/Bj_lec20.png)

## The Volume of a Box

**Claim**: |det A| is the volume of the box (parallelepiped) whose edges are the
column vectors of A. (We could equally well use the row vectors, forming a
different box with the same volume.)

If A = I, then the box is a unit cube and its volume is 1. Because this agrees
with our claim, we can conclude that the volume obeys determinant **property
1**.

If A = Q is an orthogonal matrix then the box is a unit cube in a different
orientation with volume 1 = |det Q| . (Because Q is an orthogonal matrix,
Q<sup>T</sup>Q = I and so det Q = ± 1.)

Swapping two columns of A does not change the volume of the box or (re­membering that det A = det A<sup>T</sup>) the absolute value of the determinant (**prop­erty 2**). If we show that the volume of the box also obeys property 3 we’ll have proven |det A| equals the volume of the box.

If we double the length of one column of A, we double the volume of the box formed by its columns. Volume satisﬁes **property 3(a)**.

**Property 3(b)** says that the determinant is linear in the rows of the matrix:
![Linear property of determinant](Images/determinant_linear_lec20.png)

Following figure illustrates why this should be true.

![Geometric proof of linear property of volume like determinant](Images/volume_linear_lec20.png)
