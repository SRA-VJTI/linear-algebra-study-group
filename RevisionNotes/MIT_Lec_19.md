# 19 Determinant Formulas and Cofactors

- det(`I`) = 1
- Row exchange makes sign reverse
- det is linear in each row separately

```
┃ a   b ┃    ┃ a   0 ┃   ┃ 0   b ┃
┃       ┃ =  ┃       ┃ + ┃       ┃
┃ c   d ┃    ┃ c   d ┃   ┃ c   d ┃
          
┃ a   b ┃   ┃ a   0 ┃   ┃ 0   b ┃   ┃ 0   b ┃   ┃ a   0 ┃
┃       ┃ = ┃       ┃ + ┃       ┃ + ┃       ┃ + ┃       ┃
┃ c   d ┃   ┃ c   0 ┃   ┃ c   0 ┃   ┃ 0   d ┃   ┃ 0   d ┃

┃ a   b ┃
┃       ┃ =    0      +  (-bc)    +     0     +     ad
┃ c   d ┃
```

### The cofactor formula:
- det(A) = a<sub>11</sub>C<sub>11</sub>+a<sub>12</sub>C<sub>12</sub>+...+a<sub>1n</sub>C<sub>1n</sub>
- C<sub>ij</sub> = ± det(smaller matrix with row i and col j removed)

### The big formula

<pre>
det(A) = Σ<sub>p∈permute(1...n)</sub> ±Π a<sub>ip<sub>i</sub></sub>
</pre>

### Question

- Find the determinant of F<sub>n x n</sub>.

```
    ┏                        ┓
    ┃ 1   -1                 ┃
    ┃ 1    1    -1           ┃
F = ┃      1    1    -1      ┃
    ┃                  . . . ┃
    ┃                 1    1 ┃
    ┗                        ┛
```
