This is a database of algorithms for quick Rubik's Cube mosaic assembly.

# front_face_patterns_to_algs.tsv
The `front_face_patterns_to_algs.tsv` is a table with 10M rows, divided into three files due to GitHub restrictions. Each row contains a cube face pattern along with a speed-optimal algorithm for creating this pattern on a solved Cube. It includes all `6^9 = 10'077'696` patterns, with one algorithm per pattern.

## 9-sticker pattern
A pattern is represented by nine letters, each denoting a sticker color. Stickers are listed left-to-right, top-to-bottom.

To create a pattern, hold your solved cube with the **white** face on top and the **green** face in front. Execute an algorithm. The pattern will appear on the **front** face.

## Snippets
```tsv
GGGGGGGGG	
GGGGGGGGO	Uw R2 Uw'
GGGGGGGGR	R' B' R
GGGGGGGGW	Uw R' Uw'
GGGGGGGGY	Uw R Uw'
GGGGGGGOB	L' D L' D L2
GGGGGGGOG	Uw M2 Uw'
GGGGGGGOO	L' D L
...
BBBBBBBBB	y2
BBBBBBBBG	R' U' Lw2 D R
BBBBBBBBO	Dw Lw2 Uw'
BBBBBBBBR	Lw' U' R2 Lw'
BBBBBBBBW	Rw' Uw2 Lw
BBBBBBBBY	Lw' U2 R2 Lw'
BBBBBBBGB	L2 Uw2 R2
BBBBBBBGG	U2 F' Rw2
BBBBBBBGO	F R' Uw2 L
...
RYYRYGOOY	Rw' D B Uw2 R
RYYRYGORB	D' F U' Rw F' R'
RYYRYGORG	D' Bw L' Uw R
RYYRYGORO	Uw' R U2 F' D M'
RYYRYGORR	Fw' R Uw F' L D'
RYYRYGORW	Rw F' U Fw' D R
RYYRYGORY	D' F U' Fw' Uw R
RYYRYGOWB	S' M Uw R D R
...
```

---
# top_face_8_sticker_patterns_to_algs.tsv

This file contains `6^8` = `1,679,616` rows. Each row maps a pattern defined by 8 stickers surrounding the center sticker to a move-optimal HTM algorithm to achieve it. In a pattern, stickers are denoted by their corresponding cube side instead of their color.

## 8-sticker pattern
The 8 letters represent these positions of stickers on the top face: top-left corner, top edge (above the center), top-right corner, left edge, right edge, bottom-left corner, bottom edge, and bottom-right corner.

## Examples
Example: `BUUBUBUU	L` means if you take a solved cube and apply an L move, the top-left corner of the top face of the cube will have the color of a center on the B side (red). Following that, the top edge and top-right corner will remain U-face colored (white), and so on.

```tsv
UUUUUUUU	
```
This is the first line of the file. If you apply no algorithm to the cube, all its 8 stickers will maintain the same color as the center sticker on the U face (white).

## Snippets
```tsv
UUUUUUUU	
BUUBUBUU	L
UUFUFUUF	R
UUUUULLL	F
RRRUUUUU	B
DUUDUDUU	L2
UUDUDUUD	R2
UUUUUDDD	F2
DDDUUUUU	B2
FUUFUFUU	L'
UUBUBUUB	R'
UUUUURRR	F'
LLLUUUUU	B'
BUUBULUU	U L
BUFBFBUF	R L
RUUBUBUU	D L
...
BLBLLRLF	D L' U' F' R B' L' F
FLUBLRFR	B' D2 U L2 D B' L' F
FLFLLBLD	B D' R2 B' L2 B' L' F
BLDLLDLR	U' F U F2 U2 B' L' F
LFFFFLFB	U L' D' F2 U2 B' L' F
BLBLLFLU	F U' R2 F' R2 B' L' F
BLULLBLR	D L2 R F U' B' L' F
ULBLLDLB	L' D L2 F U' B' L' F
```
