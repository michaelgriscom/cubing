# Setup Moves
These move an edge from a given position into (U) so that M2 can be applied
to swap it with (A). After undoing the setup move after M2, (A) and (U) are
now swapped. It is important that the setup move doesn't affect anything in the M slice
since the M2 touches those.

```
- (A): M2

- (B): R' U R U' M2 U R' U' R

- (C): U2 M' U2 M'

- (D): L U' L' U M2 U' L U L'

- (E): B L' B' M2 B L B'

- (F): B L2 B' M2 B L2 B'

- (G): B L B' M2 B L' B'

- (H)
    - L' B L B' M2 B L' B' L
    - U' L' U M2 U' L U

- (I): D M' U R2 U' M U R2 U' D' M2

- (J): U R U' M2 U R' U'

- (K): N/A

- (L): U' L' U M2 U' L U

- (M): B' R B M2 B' R' B

- (N):
    - R B' R' B M2 B' R B R'
    - U R U' M2 U R' U'

- (O): B' R' B M2 B' R B

- (P): B' R2 B M2 B' R2 B

- (Q): B' R B U R2 U' M2 U R2 U' B' R' B

- (R): U' L U M2 U' L' U

- (S): M2 D U R2 U' M' U R2 U' M D'

- (T): U R' U' M2 U R U'

- (U): N/A

- (V): U R2 U' M2 U R2 U'

- (W): M U2 M U2

- (X): U' L2 U M2 U' L2 U
```