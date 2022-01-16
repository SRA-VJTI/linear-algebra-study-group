
# 10 - Four fundamental subspaces

For a matrix `A`

|                                      |                                    |                                  |
| :----------------------------------: | :--------------------------------: | :------------------------------: |
|        **Column Space C(A)**         |    combination of columns of A     |  R<sup>r</sup> in R<sup>m</sup>  |
|         **Null Space N(A)**          |      all solution of `Ax = 0`      | R<sup>n-r</sup> in R<sup>n</sup> |
|    **Row Space C(A<sup>T</sup>)**    |      combination of rows of A      |  R<sup>r</sup> in R<sup>n</sup>  |
| **Left Null Space N(A<sup>T</sup>)** | all solution of A<sup>T</sup>y = 0 | R<sup>m-r</sup> in R<sup>m</sup> |

![othogonality between spaces](Images/four_fundamental_subspaces.png)

* Basis of `row` space of A ==> first `r` rows of R or A
* Basis of `column` space of A ==> pivot columns of `A`
* Basis of `null` space of A ==> special solution of A
* Basis of `left null` space of A ==> transforming `[A | I] ---> [R | E]`, look for combination of rows which give zero row
* When the rank is as large as possible, r = n or r = m or r = m = n, the matrix has a left-inverse B or a right-inverse C or a two-sided A<sup>-1</sup>
* Row spaces of A, U(echelon form) and R(reduced row echelon form) are same.
* Column spaces of A, U(echelon form) and R(reduced row echelon form) are different.

### 3x3 matrices a vector space?

<details>
  <summary>View Answer</summary>
    
  >  _Yes. Since they contain a Null vector and follow all other rules of being a vector space._
</details>
  
### What are its subspaces?

<details>
  <summary>View Answer</summary>
    
  >  _upper triangular, symmetrical, diagonal..._
</details>
