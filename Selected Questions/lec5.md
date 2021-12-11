# Lec 5 Transpose, Permutation, Spaces

1. Prove that no row/column exchange can transpose a matrix.

<details>
<summary>
Answer
</summary>
Any exchange done for elements of first row/column changes the position of first element , therefore is not a transpose.
</details>

2. A group of matrices includes AB and A^{-1} (A inverse) if it includes A and B. "Products and inverses stay in the group." Which of these sets are  groups?
   1. Lower traingular matrices L with 1s on the diagonal,
   2. symmetric matrices S,
   3. positive matrices M,
   4. Diagonal invertible matrices D,
   5. permutation matrices P.

    Invent 2 more matrix groups.

<details>
<summary>
Answer
</summary>
1 Obviously (recall gauss-jordan), 2 is not a group as two symmetric matrices have a non symmetric product (recall tanspose(AB)=transpose(B)transpose(A)), 3 is not a group as its inverse may not be a positive matrix, 4 is a group obviously, 5 is also a group.

Two more:

   1. All invertible matrices,
   2. 
<!-- $$
Q^{T}=Q^{-1}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/TV607PbQMa.svg"></div>

</details>

3. Difference between subset and subspace?

<details>
<summary>
Answer
</summary>
A subset is a set of elements only from R^{n}.
A subspace is a subset of R^{n} and also a vector space. As zero vector belongs to every subspace, it is never an empty subset.
</details>

4. Is R^{n-1} a subspace of R^{n} for n>=2 ?

<details>
<summary>
Answer
</summary>
R^{n} consists of all column vectors with n components. Hence, No as it does not contain the third component.
</details>
