## Multiplication and Inversion in matrices 
  
 - There are two ways to multiply a matrix A with a vector X 
   - Each row of A combines with X to give a component of AX.
   - Product AX is found as a combination of columns of A.
 
 - (EA)X = E(AX)
  
 - EA != AE
  
 - For two matrices A and B, AB = A[b1 b2 b3] = [Ab1 Ab2 Ab3]
  
 - The i,j entry of AB is the inner product of the ith row of A and the jth column of B.
  
   - (AB)<3, 2> = a<3, 1>*b<1, 2> + a<3, 2> * b<2, 2> + a<3, 3> * b<3, 2> + a<3, 4> * b<4, 2>
  
 - Not all matirces have inverse, inverse is impossible when AX = 0 and X != 0.
  
 - A*A^-1 = I
  
 - The inverse exists only if elimination produces n pivots in a nxm matrix.
  
 - Any square matrix cannot have two different inverses.
  
 - If A is invertible, then one and only solution to A * X = B is X = A^-1 * B
  
 - (A * B)^-1 = B^-1 * A^-1

 - Left sided, right sided and dual sided inverse matrices.
