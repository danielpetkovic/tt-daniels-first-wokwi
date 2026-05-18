<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

Only AND, OR and NOT Gates are used. 8 inputs (in0 ... in7) are used.
Activated in0 input represents the number 1. Activated in1 represents the number 2 and so on ... 
until in7 which represents the number 8.
None activated input represents the number 0.
All activated inputs represents the number 9.

## How to test

When the DIP switch for the inputs on the TinyTapeout Demo Board is used. The label of the DIP Switch input should be shown on the 7 segment display.
The label of the DIP switch is input number+1. e.g. in0 = DIP switch label 1

e.g. active input in3 should show the number 4 on the 7 segment display.
e.g. non active input should show the number 0 on the 7 segment display.
e.g. all active inputs should show the number 9 on the 7 segment display.

| input in0 ... in7 | output out0 ... out6 |
|-------------------|----------------------|
| 0 0 0 0 0 0 0 0   | 1 1 1 1 1 1 0        |
| 1 0 0 0 0 0 0 0   | 0 1 1 0 0 0 0        |
| 0 1 0 0 0 0 0 0   | 1 1 0 1 1 0 1        |
| 0 0 1 0 0 0 0 0   | 1 1 1 1 0 0 1        |
| 0 0 0 1 0 0 0 0   | 0 1 1 0 0 1 1        |
| 0 0 0 0 1 0 0 0   | 1 0 1 1 0 1 1        |
| 0 0 0 0 0 1 0 0   | 1 0 1 1 1 1 1        |
| 0 0 0 0 0 0 1 0   | 1 1 1 0 0 0 0        |
| 0 0 0 0 0 0 0 1   | 1 1 1 1 1 1 1        |
| 1 1 1 1 1 1 1 1   | 1 1 1 1 0 1 1        |

## External hardware

No external hardware should be necessary when the TinyTapout DevKit is bought. Only the Input DIP switch and 7-segment display og the TinyTapeout board is used.
Somebody could hookup a external switch (e.g. a rotary switch to avoid wrong input selections)
