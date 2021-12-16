# Lec 6 Column Space and Nullspace

1. Describe column space and nullspace of the matrices.

<!-- $$
A=
\begin{bmatrix}
     1    &  -1  \\
     0    &  0    \\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/C232a7Kgf2.svg"></div>

<!-- $$
B=
\begin{bmatrix}
     0    &  0  &   3\\
     1    &  2  &   3\\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/iQHkCCKVsQ.svg"></div>

<!-- $$
C=
\begin{bmatrix}
     0    &  0  &   0  \\
     0    &  0  &   0    \\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/BOieLAx9wJ.svg"></div>

<details>
<summary>
Answer
</summary>
C(A) spans all the positive as well as negative real numbers including 0. For N(A), x=y is the line.
C(B) spans any combination of x,y i.e. R^{2}, and N(B) is x+2y=0 passing through z=0.
C(C) is a null vector, N(C) is R^{3}.
</details>

2. If we add an extra column b to matrix A, then the column space gets larger unless _____. Give an example in which the column space gets larger and an example in which it doesn't exist. Why is Ax=b solvable exactly when the column space doesn't get larger by including b?

<details>
<summary>
Answer
</summary>

Unless b is a linear combination i.e. it's in the same space.
Example:
<!-- $$
\begin{bmatrix}
    1 & 0 \\
    0 & 1 \\
\end{bmatrix}
->
\begin{bmatrix}
    1 & 0 & 1\\
    0 & 1 & 1\\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/xFBWQ7aRdv.svg"></div> 

Column space increased:
<!-- $$
\begin{bmatrix}
    1 & 0 \\
    0 & 0 \\
\end{bmatrix}
->
\begin{bmatrix}
    1 & 0 & 1\\
    0 & 0 & 1\\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/RP2hjsu1Lb.svg"></div>

<blockquote>
</blockquote>
</details>

<!-- 3. The sum of the vectors f(x) and g(x) in F is defined to be f(g(x)), then zero vector is g(x)=x. Find the rules broken.

<details>
<summary>
Answer
</summary>

| Axiom	| Meaning |
| --- | --- |
Associativity of vector addition | 	u + (v + w) = (u + v) + w | 
Commutativity of vector addition |	u + v = v + u |
Identity element of vector addition |	There exists an element 0 ∈ V, called the zero vector, such that v + 0 = v for all v ∈ V.|
Inverse elements of vector addition	| For every v ∈ V, there exists an element −v ∈ V, called the additive inverse of v, such that v + (−v) = 0.
Compatibility of scalar multiplication with field multiplication |	a(bv) = (ab)v
Identity element of scalar multiplication |	1v = v, where 1 denotes the multiplicative identity in F.
Distributivity of scalar multiplication with respect to vector addition  |	a(u + v) = au + av
Distributivity of scalar multiplication with respect to field addition |	(a + b)v = av + bv

$$
(f+g)(x)=f(g(x)) \\
\text{What is } (g+f)(x) \text{ ?} \\
\text{What is the inverse of f ?} \\
$$

<blockquote>
</blockquote>
</details> -->
