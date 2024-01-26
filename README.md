This is a database of algorithms for quick Rubik's Cube mosaic assembly.

## Files
The `front_face_patterns_to_algs.tsv` is a table with 10M rows, divided into three files due to GitHub restrictions. Each row contains a cube face pattern along with a speed-optimal algorithm for creating this pattern on a solved Cube. It includes all `6^9 = 10'077'696` patterns, with one algorithm per pattern.

## Pattern
A pattern is represented by nine letters, each denoting a sticker color. Stickers are listed left-to-right, top-to-bottom. 
To create a pattern, hold your solved cube with the **white** face on top and the **green** face in front. Execute an algorithm. The pattern will appear on the **front** face.

## Snippet 1
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

## Snippet 2
```tsv
GGGGGGBYB	D S D
GGGGGGBYG	Uw2 F' Uw' M' Uw'
GGGGGGBYO	D' B2 S' D'
GGGGGGBYR	R' F S' D'
GGGGGGBYW	R2 Uw' Fw Rw
GGGGGGBYY	D' Bw D'
GGGGGGGBB	L2 F' L2
GGGGGGGBG	R2 D2 R2
GGGGGGGBO	D' R2 D F
GGGGGGGBR	U' L2 U F'
GGGGGGGBW	L' D2 L
GGGGGGGBY	Lw' Fw2 Rw
GGGGGGGGB	R' U R' U' R2
GGGGGGGGG	
GGGGGGGGO	Uw R2 Uw'
GGGGGGGGR	R' B' R
GGGGGGGGW	Uw R' Uw'
GGGGGGGGY	Uw R Uw'
GGGGGGGOB	L' D L' D L2
GGGGGGGOG	Uw M2 Uw'
GGGGGGGOO	L' D L
```

## Snippet 3
```tsv
RYYRYGOOW	Rw F' U F' D R
RYYRYGOOY	Rw' D B Uw2 R
RYYRYGORB	D' F U' Rw F' R'
RYYRYGORG	D' Bw L' Uw R
RYYRYGORO	Uw' R U2 F' D M'
RYYRYGORR	Fw' R Uw F' L D'
RYYRYGORW	Rw F' U Fw' D R
RYYRYGORY	D' F U' Fw' Uw R
RYYRYGOWB	S' M Uw R D R
RYYRYGOWG	S' R D R' Uw
RYYRYGOWO	R2 U F' D R2 M'
RYYRYGOWR	F U' D' B2 Lw'
RYYRYGOWW	F U' D' Lw' D2
RYYRYGOWY	y' M S Uw2 R
RYYRYGOYB	L2 U2 R' Uw F' M'
RYYRYGOYG	R' Uw Rw' D Rw2
RYYRYGOYO	D R' Uw Rw U
RYYRYGOYR	E Rw U L' F L'
RYYRYGOYW	D R' Uw L U2 Lw'
RYYRYGOYY	F D U' R' Uw2 Rw
RYYRYGRBB	R' Uw Rw U D'
```
