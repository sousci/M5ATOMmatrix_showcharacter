# M5ATOMmatrix_showcharacter
Showing character or String on M5ATOMmatrix.

## How to Installing
1. Downroad a **.m5b** file [https://github.com/sousci/M5ATOMmatrix_showcharacter/blob/main/ATOMmat_ShowString.m5b](https://github.com/sousci/M5ATOMmatrix_showcharacter/blob/main/ATOMmat_ShowString.m5b)
1. Go to [flow.m5stack.com](flow.mt5stack.com)
1. Click a "Custom" button
1. Click a "Open \*.m5b file"
1. choose and open a **ATOMmat_ShowString.m5b** in your computer
1. M5ATOMmatrix showcharacter block has been installed

## How to Use
1. First, install a "ATOM_setup" block at a head of code to load a library.
1. Install a "print" block where you want, don't forget "text" block and parameters.

### description of parameters
| parameter | description |
----|---- 
| scroll | Set the interval at which dots flow in milliseconds # recommend:100 |
| rotation | Rotate scroll derection of character or strings. <br> Clockwise when viewed from the front "0":0[deg], "1":90[deg], "2":180[deg], "3":270[deg] |
| color | set a color. The color is expressed in 24bit but it is a little hard tounderstand. <br> So we recommend a way of expressed Hexadecimal. For example, input `0xFFFFFF` * then transrate a `16777215` automatically. It means 0x**FF(red level)FF(green level)FF(blue level)**. <br> If you want to set yellow, please input `0xFFFF00`.|

## Troubleshooting
Q1. display a red "X".  
A1. Code has some trouble. Please check these.
 * Not installed "ATOM_setup" block.
 * Character or string are *NULL*.
 * Parameters incorrect. Please check next question.

Q2. Character isn't displayed.  
A2. Are parameters correct? 
Please try ;)
```
print: "test"
scroll: 100
rotation: 0
color: 16777215
```

Q3. Will you plan more function?  
A3. No. But notify please of find bugs:)
