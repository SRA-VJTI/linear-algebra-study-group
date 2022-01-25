# 15 - Projections into subspaces

### The basics of projection
![Projection image](./Images/MIT_15_projection.png)

### Defining a basic formula for projecting b onto a line formed by a single vector.
![Projection derivation example](./Images/MIT_15_basic.png)

- Let `p` be the projection of `b` onto the line going through `a`.
- Since `p` is at the shortest distance possible from `b`, the line joining them must be perpendicular to the line formed by multiples of `a`.
- Therefore, if `e = b - p`, then e must be perpendicular to a.
- Now `p` is a scalar multiple of `a`, so let `p = ax` with x being a scalar.
- We get a<sup>T</sup> (b- ax) = 0.
- Rearranging and substituting x, p = a(a<sup>T</sup>  . b / a<sup>T</sup>  . a)
- By using the associative law, we see that p = (a . a<sup>T</sup> / a<sup>T</sup>  . a)b with the first bracket being known as the projection matrix.

### Applying this formula to approximating Ax = b when there are no solutions to it.

- Instead of solving `Ax=b` we solve `Ax=p`, where `p` is the projection of `b` onto the coloumn space of A.
- So we first find `p` and then predict `x` as the closest answer.
- So in this case `b - p` i.e. `b - Ax` has to be perpendicular to the plane with basis vectors as `a1` and `a2` (this is an example of a 2-dimensional subspace)
- So, a1<sup>T</sup> (b - Ax) = 0 and a2<sup>T</sup> (b - Ax) = 0, combining which vertically gives, A<sup>T</sup> (b - Ax) = 0.
- Rearranging and substituting, we get A<sup>T</sup> Ax = A<sup>T</sup> b, p= A (A<sup>T</sup> A)^-1 A<sup>T</sup> b

### Some important properties of P (the projecting matrix)'
- P<sup>T</sup> = P
- P . P  = P
