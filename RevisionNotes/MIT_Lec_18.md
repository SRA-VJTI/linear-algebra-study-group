# Properties of determinants

## Introduction

- The determinant is a number associated with any square matrix.
- Denoted as det A or |A|.
- The matrix is invertible exactly when the determinant is non-zero.

## Properties

### Property 1 :

- det(I) = 1

### Property 2 :

- Row exchange reverses the sign of determinant
- From above a permutation matrix determinant could be 1 or -1.
- It is dependent on the number row exchanges.
- If even then 1
- Else odd then -1.

### Property 3 :

A)

- Multiplier from row can be taken common and determinant will be multiplied by the same.
<pre>
   | ta tb |  =   t| a b | 
   |  c  d |       | c d |


</pre>
B) 
- Determinant can be split with respect to one row.
- It behaves like a linear function on the rows of the matrix.
<pre>
   | a+e b+f |  =    | a b | + | e f |
   |  c   d |        | c d |   | c d |
       
</pre>
##### **All other properties can be derived from above 3 properties.**

### Property 4 :

- If two rows of a matrix are equal, its determinant is zero. (From property 2).

### Property 5 :

- Subtracting l x row<sub>i</sub> from row<sub>k</sub> the determinant doesn't change. (From property 3 and 4)

### Property 6 :

- If A has a row that is all zeros, then det A = 0. (From property 3(a) substituting t = 0).

### Property 7 :

- The determinant of a triangular matrix is the product of the diagonal entries (pivots) d1, d2, ..., dn.
- Reduce using property 5.
- Factor out constants of diagonals by property 3.
- From property 1 determinant would be product of these factors as determinant of identity matrix is 1.

### Property 8 :

- det(A) = 0 implies A is singular
- det(A) ≠ 0 implies A is invertible
- If A is singular then through elimanation we would get row of Zeroes then using property 6.
- Otherwise we would pivots d1, d2, ...., dn and then using property 7.
- Therefore, there are only 2 above cases of this property.
- Determinant is fair test for invertibility.

### Property 9 :

- det(AB) = det(A)\*det(B)
- Other derivatives from this:
- det(A<sup>-1</sup>) = 1 / det(A)
- det(A<sup>n</sup>) = (det(A))<sup>n</sup>
- det(c\*A) = c<sup>n</sup>det(A) [Considering nXn matrix].

### Property 10 :

- det(A<sup>T</sup>) = det(A)
<pre>
    |A<sup>T</sup>| = |A|
    |U<sup>T</sup>L<sup>T</sup>| = |LU|
    |U<sup>T</sup>|.|L<sup>T</sup>| = |LU|
    Product(diag of U<sup>T</sup>).Product(diag of L<sup>T</sup>) = Product(diag of L).Product(diag of U)
    This is true.


</pre>
- Also, determinant of skew-symmetric matrix of odd order = 0.

### Some points :

- All above properties also holds for column.
- Result of an odd number of row exchanges (odd permutation) can never be the same as the result of an even number of row exchanges (even permutation)
