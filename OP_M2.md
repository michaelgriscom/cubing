# Notation
- (A), (B)...(X) represent stickers on the cube as indexed through Speffz notation
- *(A) represents the 'true' position that the sticker at (A) should occupy in a solved cube, **(A) represents the true position for the sticker that is in (A)'s true position.

# Method
## Memo
Letter pairs can be memorized via [the Person/Object method](PO_Memo.md)

### Edge Memo
- Start at corner (A), then locate *(A), **(A), etc until the buffer cube is reached [via (A), (E), or (R)]
    - While not all edges have been traversed, locate a new unvisited corner (e.g., (C)) and treat it like A, continuing on to *(C), **(C), etc until (C) is reached
- You will have a string of characters with length <= 8. Pair up the letters.

### Corner Memo
- Start at (U), then locate *(U), **(U), etc until the buffer cube is reached [via (U) or (K)]
    - While not all edges have been traversed, locate a new unvisited corner (e.g., (C)) and treat it like A, continuing on to *(C), **(C), etc until (C) is reached
- If you encounter a (C) or (W) on an even number, then switch to the other letter in the pair. Likewise for the (I)/(S) pair
- You will have a string of characters with length <= 12. Pair up the letters

Note whether the memo strings are odd length, if so a parity fix will need to be
performed. If the strings have unequal parity then one of them was done incorrectly.

## Execution
- Execute [M2 Edges](M2_Edges.md)
- If the memo was of an odd length, perform the parity fix:
    - `(D' L2 D) M2 (D' L2 D)`
- Execute [OP Corners](OP_Corners.md)

# References
- For setup moves and parity algorithm [[NoahCubes] How to Solve a Rubik's Cube Blindfolded: Part 3](https://www.youtube.com/watch?v=o49SnZhr2oM)
- Y Perm [Old Pochmann - Corner and Edge Method](https://www.speedcubereview.com/blind-solving-algorithms.html)