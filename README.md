## code 128

The Code-128 Fonts i found on the internet had no Start/Stop Codes or where generally broken. So i created this repository. It contains code 128 fonts in .svg, .ttf and .woff format.

The fonts are available in 5 different Sizes: S,M,L,XL,XXL. They differ in height vs. width ratio.

* fonts/code128_S(.svg, .ttf, .woff)
* fonts/code128(.svg, .ttf, .woff)
* fonts/code128_L(.svg, .ttf, .woff)
* fonts/code128_XL(.svg, .ttf, .woff)
* fonts/code128_XXL(.svg, .ttf, .woff)

see the font in action in the [Live Example](https://cdn.rawgit.com/Holger-Will/code128/master/examples/generator.html)

In CSS you can use it like this for example:

    @font-face { font-family: 'code128'; src: url('../fonts/code128.ttf'); }
    .barcode { font-family: code128; font-size:50px }

and in your .html:

    <span class="barcode">abcde</span>

**You can not scan code that you output like this!**

Details can be found under [Generate Codes](#generating-codes)

# Tools and Information

the general information and code table was taken from the Wikipedia Article on [Code 128](https://en.wikipedia.org/wiki/Code_128)
The code table is then turned to .json, and the .json into an .svg font.
I used the ecxellent tools [svg2ttf](https://github.com/fontello/svg2ttf) and [ttf2woff](https://github.com/fontello/ttf2woff) by [fontello](https://github.com/fontello) to convert the font to ttf and woff.

And the fantastic [font dragr](http://labs.thecssninja.com/font_dragr/) by Ryan Seddon for initial testing.

In the root folder there is a bash script called generate which you can use to regenerate all fonts (in case you want to specify your own hight to width ratio)

see the font in action in the [Live Example](https://cdn.rawgit.com/Holger-Will/code128/master/examples/generator.html)


# Code Table

| Code | A | B | C | ASCII | Symbol | Bars and Spaces | Weights |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | SPACE | SPACE | 00 | 32,212,252 |   | 11011001100 | 212222 |
| 1 | ! | ! | 01 | 33 | ! | 11001101100 | 222122 |
| 2 | " | " | 02 | 34 | " | 11001100110 | 222221 |
| 3 | # | # | 03 | 35 | # | 10010011000 | 121223 |
| 4 | $ | $ | 04 | 36 | $ | 10010001100 | 121322 |
| 5 | % | % | 05 | 37 | % | 10001001100 | 131222 |
| 6 | & | & | 06 | 38 | & | 10011001000 | 122213 |
| 7 | ' | ' | 07 | 39 | ' | 10011000100 | 122312 |
| 8 | ( | ( | 08 | 40 | ( | 10001100100 | 132212 |
| 9 | ) | ) | 09 | 41 | ) | 11001001000 | 221213 |
| 10 | * | * | 10 | 42 | * | 11001000100 | 221312 |
| 11 | + | + | 11 | 43 | + | 11000100100 | 231212 |
| 12 | , | , | 12 | 44 | , | 10110011100 | 112232 |
| 13 | - | - | 13 | 45 | - | 10011011100 | 122132 |
| 14 | . | . | 14 | 46 | . | 10011001110 | 122231 |
| 15 | / | / | 15 | 47 | / | 10111001100 | 113222 |
| 16 | 0 | 0 | 16 | 48 | 0 | 10011101100 | 123122 |
| 17 | 1 | 1 | 17 | 49 | 1 | 10011100110 | 123221 |
| 18 | 2 | 2 | 18 | 50 | 2 | 11001110010 | 223211 |
| 19 | 3 | 3 | 19 | 51 | 3 | 11001011100 | 221132 |
| 20 | 4 | 4 | 20 | 52 | 4 | 11001001110 | 221231 |
| 21 | 5 | 5 | 21 | 53 | 5 | 11011100100 | 213212 |
| 22 | 6 | 6 | 22 | 54 | 6 | 11001110100 | 223112 |
| 23 | 7 | 7 | 23 | 55 | 7 | 11101101110 | 312131 |
| 24 | 8 | 8 | 24 | 56 | 8 | 11101001100 | 311222 |
| 25 | 9 | 9 | 25 | 57 | 9 | 11100101100 | 321122 |
| 26 | : | : | 26 | 58 | : | 11100100110 | 321221 |
| 27 | ; | ; | 27 | 59 | ; | 11101100100 | 312212 |
| 28 | < | < | 28 | 60 | < | 11100110100 | 322112 |
| 29 | = | = | 29 | 61 | = | 11100110010 | 322211 |
| 30 | > | > | 30 | 62 | > | 11011011000 | 212123 |
| 31 | ? | ? | 31 | 63 | ? | 11011000110 | 212321 |
| 32 | @ | @ | 32 | 64 | @ | 11000110110 | 232121 |
| 33 | A | A | 33 | 65 | A | 10100011000 | 111323 |
| 34 | B | B | 34 | 66 | B | 10001011000 | 131123 |
| 35 | C | C | 35 | 67 | C | 10001000110 | 131321 |
| 36 | D | D | 36 | 68 | D | 10110001000 | 112313 |
| 37 | E | E | 37 | 69 | E | 10001101000 | 132113 |
| 38 | F | F | 38 | 70 | F | 10001100010 | 132311 |
| 39 | G | G | 39 | 71 | G | 11010001000 | 211313 |
| 40 | H | H | 40 | 72 | H | 11000101000 | 231113 |
| 41 | I | I | 41 | 73 | I | 11000100010 | 231311 |
| 42 | J | J | 42 | 74 | J | 10110111000 | 112133 |
| 43 | K | K | 43 | 75 | K | 10110001110 | 112331 |
| 44 | L | L | 44 | 76 | L | 10001101110 | 132131 |
| 45 | M | M | 45 | 77 | M | 10111011000 | 113123 |
| 46 | N | N | 46 | 78 | N | 10111000110 | 113321 |
| 47 | O | O | 47 | 79 | O | 10001110110 | 133121 |
| 48 | P | P | 48 | 80 | P | 11101110110 | 313121 |
| 49 | Q | Q | 49 | 81 | Q | 11010001110 | 211331 |
| 50 | R | R | 50 | 82 | R | 11000101110 | 231131 |
| 51 | S | S | 51 | 83 | S | 11011101000 | 213113 |
| 52 | T | T | 52 | 84 | T | 11011100010 | 213311 |
| 53 | U | U | 53 | 85 | U | 11011101110 | 213131 |
| 54 | V | V | 54 | 86 | V | 11101011000 | 311123 |
| 55 | W | W | 55 | 87 | W | 11101000110 | 311321 |
| 56 | X | X | 56 | 88 | X | 11100010110 | 331121 |
| 57 | Y | Y | 57 | 89 | Y | 11101101000 | 312113 |
| 58 | Z | Z | 58 | 90 | Z | 11101100010 | 312311 |
| 59 | [ | [ | 59 | 91 | [ | 11100011010 | 332111 |
| 60 | \ | \ | 60 | 92 | \ | 11101111010 | 314111 |
| 61 | ] | ] | 61 | 93 | ] | 11001000010 | 221411 |
| 62 | ^ | ^ | 62 | 94 | ^ | 11110001010 | 431111 |
| 63 | _ | _ | 63 | 95 | _ | 10100110000 | 111224 |
| 64 | NUL | \` | 64 | 96 | \` | 10100001100 | 111422 |
| 65 | SOH | a | 65 | 97 | a | 10010110000 | 121124 |
| 66 | STX | b | 66 | 98 | b | 10010000110 | 121421 |
| 67 | ETX | c | 67 | 99 | c | 10000101100 | 141122 |
| 68 | EOT | d | 68 | 100 | d | 10000100110 | 141221 |
| 69 | ENQ | e | 69 | 101 | e | 10110010000 | 112214 |
| 70 | ACK | f | 70 | 102 | f | 10110000100 | 112412 |
| 71 | BEL | g | 71 | 103 | g | 10011010000 | 122114 |
| 72 | BS | h | 72 | 104 | h | 10011000010 | 122411 |
| 73 | HT | i | 73 | 105 | i | 10000110100 | 142112 |
| 74 | LF | j | 74 | 106 | j | 10000110010 | 142211 |
| 75 | VT | k | 75 | 107 | k | 11000010010 | 241211 |
| 76 | FF | l | 76 | 108 | l | 11001010000 | 221114 |
| 77 | CR | m | 77 | 109 | m | 11110111010 | 413111 |
| 78 | SO | n | 78 | 110 | n | 11000010100 | 241112 |
| 79 | SI | o | 79 | 111 | o | 10001111010 | 134111 |
| 80 | DLE | p | 80 | 112 | p | 10100111100 | 111242 |
| 81 | DC1 | q | 81 | 113 | q | 10010111100 | 121142 |
| 82 | DC2 | r | 82 | 114 | r | 10010011110 | 121241 |
| 83 | DC3 | s | 83 | 115 | s | 10111100100 | 114212 |
| 84 | DC4 | t | 84 | 116 | t | 10011110100 | 124112 |
| 85 | NAK | u | 85 | 117 | u | 10011110010 | 124211 |
| 86 | SYN | v | 86 | 118 | v | 11110100100 | 411212 |
| 87 | ETB | w | 87 | 119 | w | 11110010100 | 421112 |
| 88 | CAN | x | 88 | 120 | x | 11110010010 | 421211 |
| 89 | EM | y | 89 | 121 | y | 11011011110 | 212141 |
| 90 | SUB | z | 90 | 122 | z | 11011110110 | 214121 |
| 91 | ESC | { | 91 | 123 | { | 11110110110 | 412121 |
| 92 | FS | \| | 92 | 124 | \| | 10101111000 | 111143 |
| 93 | GS | } | 93 | 125 | } | 10100011110 | 111341 |
| 94 | RS | ~ | 94 | 126 | ~ | 10001011110 | 131141 |
| 95 | US | DEL | 95 | 200,240 | È | 10111101000 | 114113 |
| 96 | FNC 3 | FNC 3 | 96 | 201,241 | É | 10111100010 | 114311 |
| 97 | FNC 2 | FNC 2 | 97 | 202,242 | Ê | 11110101000 | 411113 |
| 98 | Shift B | Shift A | 98 | 203,243 | Ë | 11110100010 | 411311 |
| 99 | Code C | Code C | 99 | 204,244 | Ì | 10111011110 | 113141 |
| 100 | Code B | FNC 4 | Code B | 205,245 | Í | 10111101110 | 114131 |
| 101 | FNC 4 | Code A | Code A | 206,246 | Î | 11101011110 | 311141 |
| 102 | FNC 1 | FNC 1 | FNC 1 | 207,247 | Ï | 11110101110 | 411131 |
| 103 | Start Code A |  |  | 208,248 | Ð | 11010000100 | 211412 |
| 104 | Start Code B |  |  | 209,249 | Ñ | 11010010000 | 211214 |
| 105 | Start Code C |  |  | 210,250 | Ò | 11010011100 | 211232 |
| 106 | Stop (7 bars/spaces) |  |  | 211,251 | Ó | 1100011101011 | 2331112 |


# Generating Codes

you can generate working scannable codes with the help of tools/generator.js

    var generator = new Code128Generator()
    var code = generator.getCode(txt)

the result is an ascii code, that when rendered with a code 128 Font will display a scannable  Code-128 Code.
please be aware that this is not a full blown encoder. It uses standard Code B encodings (see code table). No optimizations will be performed.
