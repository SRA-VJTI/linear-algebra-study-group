# Practice Problems

### 1. Which of the following is true for any matrix A?  
**_NOTE_: dim(C(A)) ==> dimension of column space of A, dim(N(A)) ==> dimension of null space of A**  
* rank(A) > dim(C(A))
* dim(C(A)) = dim(N(A))
* dim(N(A)) + dim(C(A)) = dimension of whole vector space
* None

<details>
  <summary>View Answer</summary>
    
  >  _dim(N(A)) + dim(C(A)) = dimension of whole vector space_
</details>

### 2. Let A, B, C, D be n × n matrices. If ABCD = 1, then B<sup>-1</sup>?
* D<sup>-1</sup>C<sup>-1</sup>A<sup>-1</sup>
* CDA
* ADC
* None
* Insufficient information

<details>
  <summary>View Answer</summary>
    
  >  _Insufficient information. Since it is not given that the matrices are invertible. If invertible the answer would be ==> CDA_
</details>

### 3. Find a transformation matrix in 3D space, that first rotates the space about X axis by 270<sup>o</sup>, then rotates the resulting space about its Y axis by 90<sup>o</sup> and finally rotates the resulting space about its Z axis by 180<sup>o</sup> (All rotations in clockwise direction)

<details>
  <summary>View Answer</summary>
    
  Let A ==> Rotation about X by -270<sup>o</sup>  
      B ==> Rotation about Y by -90<sup>o</sup>  
      C ==> Rotation about Z by -180<sup>o</sup> since clockwise*  
  A = 
  
  |   1   |   0   |   0   |
  | :---: | :---: | :---: |
  |   0   |   0   |   1   |
  |   0   |  -1   |   0   |


  B = 
  

  |   0   |   0   |  -1   |
  | :---: | :---: | :---: |
  |   0   |   1   |   0   |
  |   1   |   0   |   0   |


  C = 
  
  |  -1   |   0   |   0   |
  | :---: | :---: | :---: |
  |   0   |  -1   |   0   |
  |   0   |   0   |   1   |

  Resultant transformation = **C x B x A**  
  Think why preorder multiplication?
</details>

### 4. Does all natural numbers in range (0, ∞) form a vector space or sub space? Justify

<details>
  <summary>View Answer</summary>
    
  >  _No, Since zero vector is not present_
</details>

### 5. Does all natural numbers in range (-∞, 0] form a vector space or sub space? Justify

<details>
  <summary>View Answer</summary>
    
  >  _For any space to be a vector space/subspace, there should be closure i.e resultant vector after 
  linear transformation should lie in same space. But here the resultant can be positive and hence
  the answer is NO_
</details>

### 6. Does all 2D matrices form a vector space? Justify

<details>
  <summary>View Answer</summary>
    
  >  _Yes_
</details>

### 7. A transformation matrix squishes 4D space into line, what is the rank of that matrix?
* 0
* 1
* 2
* 3
* 4

<details>
  <summary>View Answer</summary>
    
  >  _1 (Since line)_
</details>

### 8. What matrix can rotate 2D space by 60degree in anticlockwise direction?
<details>
  <summary>View Answer</summary>
  <table>
  <tr> <td>cos(60 deg)   </td> <td> -sin(60 deg)</td>   </tr>
  <tr> <td>sin(60 deg)   </td> <td> cos(60 deg)</td>   </tr>
  </table>
    
</details>

### 9. How many basis exists for a 4D vector space and how many vectors are there in that basis

<details>
  <summary>View Answer</summary>
    
  >  _Infinite number of basis, each basis consists of 4 vectors_
</details>

### 10. Basis1 -->  \[[1 0], [0, 1]], Basis2 --> \[[0 1], [1, 0]]. If a vector in basis1 is given as [3, 3], what it will be in basis 2?
<details>
  <summary>View Answer</summary>
  [3,3]
    
</details>

### 11. Find the determinant of this matrix
<table>
<tr><td>2</td><td>.</td> <td>1</td><td>9</td><td>5</td></tr>
<tr><td>-4</td> </tr>
<tr><td>7</td></tr>
</table>

<details>
  <summary>View Answer</summary>

  > _0
    
</details>

### 12. Prove that determinant of the matrix given below is , det(A) = ad - bc

|     |     |
| --- | --- |
| a   | b   |
| c   | d   |

<details>
  <summary>View Answer</summary>
    
  ![det-proof](Images/Det_Proof.png)  
  Area of resultant parallelogram = (a+b)x(c+d) - [2bc + ac/2 + ac/2 + bd/2 + bd/2]
</details>


### 13. Find Eigen values and eigen vectors of A 
|     |     |
| --- | --- |
| 0   | 1   |
| -2  | -3 |
<details>
  <summary>View Answer</summary>

    > Eigen Values: -1 , -2
    > Eigen Vectors: [t,-t] , [t, -2t]
</details>

### 14. Find the inverse of the below matrix and Justify
|     |     |    |
| --- | --- | ---|
| 5   | -2  | 4  |
| -2  | 1   | 1  |
| 4   | 1   | 0  |
<details>
  <summary>View Answer</summary>

    
</details>

### 15. Find the inverse of the below matrix and Justify
|     |     |    |
| --- | --- | ---|
| 1   | 2   | 1  |
| 5   | 2   | 4  |
| 4   | 0   | 3  |
<details>
  <summary>View Answer</summary>
    
</details>