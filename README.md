This is a database of algorithms for quick Rubik's Cube mosaic assembling.

## Files
The `front_face_patterns_to_algs.tsv` is a 10M rows table split into 3 files because of GitHub restrictions. Each row contain a cube face pattern along with a speed-optimal algorithm for creating this pattern on a solved Cube. It includes all `6^9 = 10'077'696` patterns with one alg per pattern.

## Pattern
A pattern is represented with 9 letters, each denoting a sticker color. Stickers are listed left-to-right, top-to-bottom.
To create a pattern, hold your solved cube with **white** face on top and **green** face on front. Execute an algorithm. The pattern will appear on the **front** face.

## Snippet
```tsv
BBBBBBBBB	y2
BBBBBBBBG	R' U' Lw2 D R
BBBBBBBBO	Dw Lw2 Uw'
BBBBBBBBR	Lw' U' R2 Lw'
BBBBBBBBW	Rw' Uw2 Lw
BBBBBBBBY	Lw' U2 R2 Lw'
BBBBBBBGB	L2 Uw2 R2
BBBBBBBGG	U2 F' Rw2
BBBBBBBGO	F R' Uw2 L
BBBBBBBGR	F' R' Uw2 L
BBBBBBBGW	R' Uw2 L
BBBBBBBGY	L' U2 Rw2 L'
BBBBBBBOB	Dw R2 L2 Uw'
BBBBBBBOG	L' U L' U Rw2
BBBBBBBOO	Dw L2 Uw'
BBBBBBBOR	F2 Dw L2 Uw'
BBBBBBBOW	Dw L2 R' Uw'
BBBBBBBOY	Dw R L2 Uw'
BBBBBBBRB	Dw' R2 L2 Uw
BBBBBBBRG	L' F L' U' Rw2
BBBBBBBRO	U R U' R Lw2
BBBBBBBRR	L' U' Rw2 L'
```
