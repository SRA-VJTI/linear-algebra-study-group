# Lec 4 A=LU

1. Solve the system AX=b with Lc=b

<!-- $$
A=
\begin{bmatrix}
     1    &  0   &  0   \\
    -1    &  1   &  0   \\
     0    & -1   &  1   \\
\end{bmatrix}
\begin{bmatrix}
    d_{1} & & \\
     & d_{2} &  \\
     & & d_{3} \\
\end{bmatrix}
\begin{bmatrix}
     1    &  -1  &  0   \\
     0    &  1   &  -1   \\
     0    &  0   &  1   \\
\end{bmatrix}
\\
\text{}\\
\text{and}
\text{}\\
\text{}\\
\begin{bmatrix}
     1    &  0   &  0   \\
    -1    &  1   &  0   \\
     0    & -1   &  1   \\
\end{bmatrix}
\begin{bmatrix}
    c_{1} \\
    c_{2} \\
    c_{3} \\
\end{bmatrix}
=
\begin{bmatrix}
    0 \\
    0 \\
    1 \\
\end{bmatrix}
=b
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/eBK58mKnNF.svg"></div>

<details>
<summary>
Answer
</summary>

<!-- $$
A=LDU    \\
\text{}\\
\text{and } AX=b    \\
\text{}\\
\therefore LDUX=b   \\
\text{}\\
\text{On comparing with}\\
Lc=b    \\
\text{}\\
\text{We get,} \\
c=DUX
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/t556EubS4X.svg"></div>
<br>

<!-- $$
\therefore
c=
\begin{bmatrix}
    0 \\
    0 \\
    1 \\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/Due43I6LxE.svg"></div>
<br>

<!-- $$
\therefore
\begin{bmatrix}
    d_{1} & & \\
     & d_{2} &  \\
     & & d_{3} \\
\end{bmatrix}
\begin{bmatrix}
     1    &  -1  &  0   \\
     0    &  1   &  -1   \\
     0    &  0   &  1   \\
\end{bmatrix}
X=
\begin{bmatrix}
    0 \\
    0 \\
    1 \\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/coVUDaXiqe.svg"></div>
<br>

<!-- $$
\therefore
\begin{bmatrix}
     1    &  1  &  1   \\
     0    &  1   &  1   \\
     0    &  0   &  1   \\
\end{bmatrix}
D^{-1}
D
U
X
=
\begin{bmatrix}
     1    &  1  &  1   \\
     0    &  1   &  1   \\
     0    &  0   &  1   \\
\end{bmatrix}
D^{-1}
b
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/EeXK5Ix9Sq.svg"></div>

<!-- $$
\therefore
X
=
\begin{bmatrix}
     1/d_{3}  \\
     1/d_{3}   \\
     1/d_{3}   \\
\end{bmatrix}
$$ --> 

<br>
<div align="center"><img style="background: white;" src="../assets/svg/NPWboNzxQ3.svg"></div>

<blockquote>
</blockquote>
</details>

1. Compute L and U for the symmetric matrix

<!-- $$
A=
\begin{bmatrix}
    a    &  a   &  a    &   a   \\
    a    &  b   &  b    &   b   \\
    a    &  b   &  c    &   c   \\
    a    &  b   &  c    &   d   \\
\end{bmatrix}
$$ --> 

<div align="center"><img style="background: white;" src="../assets/svg/aCv0V2h2if.svg"></div>
<br>

<details>
<summary>
Answer
</summary>

<!-- $$
\begin{bmatrix}
    1    &  0   &  0    &   0   \\
    -1    &  1   &  0    &   0   \\
    -1    &  -1   &  1    &   0   \\
    -1    &  -1   &  -1    &   1   \\
\end{bmatrix}
A
=
\begin{bmatrix}
    a    &  a   &  a    &   a   \\
    0    &  b-a   &  b-a    &   b-a   \\
    0    &  0   &  c-b    &   c-b   \\
    0    &  0   &  0    &   d-c   \\
\end{bmatrix}\\
\text{}\\
\therefore
A
=
\begin{bmatrix}
    1    &  0   &  0    &   0   \\
    1    &  1   &  0    &   0   \\
    1    &  1   &  1    &   0   \\
    1    &  1   &  1    &   1   \\
\end{bmatrix}
\begin{bmatrix}
    a    &  a   &  a    &   a   \\
    0    &  b-a   &  b-a    &   b-a   \\
    0    &  0   &  c-b    &   c-b   \\
    0    &  0   &  0    &   d-c   \\
\end{bmatrix}
$$ --> 

<br>
<div align="center"><img style="background: white;" src="../assets/svg/VzltJa1maF.svg"></div>

<blockquote>
</blockquote>
</details>
