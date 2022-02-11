# 17 - Orthogonal basis, Orthogonal square matrix (Q), Gram-Schmidt (A --> Q)

* Orthonormal vector - 
  * q<sub>i</sub><sup>T</sup>q<sub>j</sub> = 0, if i is not equal to j
  * q<sub>i</sub><sup>T</sup>q<sub>j</sub> = 1, if i is equal to j

  That is they all have (normal) length 1 and are perpendicular (ortho) to each other. 


* Q<sup>T</sup>Q = I {Q<sub>mxn</sub>: for all values of m,n } <br>
 ![img](Images/QtQ.png) 
* BTW, QQ<sup>T</sup> != I , for every Q<sub>mxn</sub> 

* QQ<sup>T</sup> = I {Q<sub>mxn</sub>: m = n} (i.e. a square matrix)

* since Q<sup>T</sup> is both left and right inverse, Q<sup>T</sup> is complete inverse of Q, when Q is a square matrix
* if Q is square - Q<sup>T</sup> = Q<sup>-1</sup>
> Example:
> <b>A Permutation matrix P</b> <br>
>    \[[0,1,0], <br>
>     [0,0,1], <br>
>     [1,0,0]] <br>
> This is an orthogonal matrix of dim 3x3. Square, hence, orthogonal matrix. <br>
> .........\[[0,0,1],<br>
> P<sup>-1</sup> = [1,0,0],<br>
> .........[0,1,0]] <br>
> <b>P<sup>-1</sup> = P<sup>T</sup></b>

* Significance of square orthonormal matrix -
    * A square orthonormal matrix Q is called an <b> orthogonal matrix </b>.
    * Q<sub>mxm</sub> i.e. dimension of vector(m) of column vectors = number of basis vectors(n) of column space
    * square orthonormal matrix Q is composed of all basis vectors of the vector space
    * all columns are independent, hence, full rank -> inverse exists. 


* Why orthonormal Matrix ? What is made easier?
    * never overflow / underflow 
        * Overflow - extremely large exponents - higher powers towards infi e.g. 10<sup>10000</sup>
        * Underflow - extremely smaller values - lower powers towards 0 e.g. 10<sup>- 10000</sup> 
        * how ? 

  * Projection matrix calculation: P = Q(Q<sup>T</sup>Q)<sup>-1</sup>Q<sup>T</sup> = QQ<sup>T</sup>
  * P = I if Q is square ( Q<sup>T</sup> = Q<sup>-1</sup>)
    * intuitive significance? 
    Q is basis matrix of entire vector space. So asking for projection of a vector in its entire vector space is the same vector itself. 💁‍♀️
  * Many equations become trivial when using matrix with orthonormal columns. If our basis is orthonormal, the projection component x<sub>i</sub>ˆ is just q<sub>i</sub> <sup>T</sup>b because A<sup>T</sup>Axˆ = A<sup>T</sup>b becomes xˆ = Q<sup>T</sup>b.
    * example
* Examples
![example](Images/orthoEg.png) <br>
    * Rotation matrices
    * Hadamard matrices: Combinations of \[[1,1],[1,-1]]

* Orthonormal vectors are always independent. Easy to prove. Try it. 
> <details>
>  <summary>Hint 1</summary>
>    AX = O
> </details> 
> <details>
>  <summary>Hint 2</summary>
>    S.T. if QX = O then X = O
> </details> 
> <details>
>  <summary>Proof</summary>
> QX = O <br>
> Q<sup>T</sup>QX = O  <br>
> IX = O  <br>
> X = O 
> </details> 
* Gram-Schmidt (make matrix A to Q) <br>
  ![Diagram](Images/gramSchmidt.png)
  * take independent vectors of A - a, b
  * Make them orthogonal by projection
  * Normalize for orthonormal
  * For multiple vectors - one by one take vector and remove components of previous vectors from it
  * A = QR : Q is Orthonormal matrix, R is upper triangular 


