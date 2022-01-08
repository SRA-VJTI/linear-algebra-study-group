## Complete Solution for Ax=b, Reduced Row Echlon Form R

### Solving Ax=b
The equations are:<br>
  x1 + 2x2 + 2x3 + 2x4 = b1<br>
 2x1 + 4x2 + 6x3 + 8x4 = b2<br>
 3x1 + 6x2 + 8x3 + 10x4 =b3<br><br>
The augmented matrix would be:<br>
![Augmented matrix](Images/3x4_aug_mat.jpg)
<br>After performing row operations on the matrix, you get the reduced form as:<br>
![Reduced matrix](Images/3x4_aug_mat_red.jpg)
<br>Considering b as 1,5,6 we get the matrix as:<br>
![Reduced matrix1](Images/3x4_aug_mat_red1.jpg)

<br>

### Solvability
Determining whether Ax=b is solvable or no.<br>
Ax=b is solvable when b is in the column space of A C(A).
If a combination of rows of A gives zero row then same combination of entries of b must give 0.<br>
In this case, the matrix is solvable and so lets find the solution.<br>

### Complete Solution for Ax=b
In order to find the complete solution for Ax=b, we need to find the particular solution.<br>
X<sub>particular</sub> : In order to find X<sub>particular</sub>, we need to set the free variables to 0 and then solve for the pivot variables.<br>
In our example we set x2=0 and x4=0,<br>
we get,<br>
x1 + 2x3 =1<br>
2x3 = 3<br>
![x-particular](Images/x_pat.jpg)

<br>
X<sub>null space</sub> : In order to find X<sub>null space</sub>, we need to set the free varialbes as 0 and 1.<br>
X<sub>complete</sub> = X<sub>particular</sub> + X<sub>null space</sub> <br> 

![x-complete](Images/x_com.jpg)

<br>

### Rank of a matrix
Rank of a matrix is determined by :
* Number of pivot
* Number of independent columns/rows
* Dimension of column space  <br>
r <= `max`(m, n) where,
 m = rows, n = columns  <br>

|   Condition    |   Solution    |                    Comment                    |
| :------------: | :-----------: | :-------------------------------------------: |
|   r = n < m    |    0 or 1     | No free variables. Hence, null space is empty |
|   r = m < n    |   Infinite    |   Every row has pivot, `n-r` free variables   |
|   r = m = n    |    Unique     |               Invertible matrix               |
| r < m && r < n | 0 or Infinite |                depends on `b`                 |

                                                                                                                   








