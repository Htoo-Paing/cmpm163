# Lab 4 for CMPM 163
Introduction to Textures and Normal Maps.

Google Drive link to video:
https://drive.google.com/open?id=1oGbFcfU0_hMgiH2y3dcdaUsEk2BmQkKt

## Writeup

Top Left: Followed baseline instructions of Part 1. Has no normal map.

Top Middle: Followed baseline instructions of Part 1. Has a normal map.

Top Right: Followed baseline instructions of Part 1. Uses a different texture and normal map from the top left and top middle counterparts.

Bottom Left: Followed baseline instructions of Part 2. Uses a custom written vertex and fragment shader.

Bottom Right: Uses a custom written vertex and fragment shader, as well as a tileable texture. To achieve the tiling, the texture was multiplied by a [2, 2] vector in the fragment shader while the 2D texture had its wrapping property changed to repeat using THREE.js's built-in wrapS and wrapT functions.

##Questions

If we assume that we want (0, 0) to map to (0, 0):  
a) ⌊u * 8⌋ = x  
b) ⌊(1 - v) * 8⌋ = y  
c) (u , v) = (0.375, 0.25)  
⌊0.375 * 8⌋ = 3  
⌊(1 - 0.25) * 8⌋ = 6  
(x, y) = (3, 6) = [White]

If we assume that we want the provided images to map to each other unchanged with the inverted y axis:  
a) ⌊u * 8⌋ = x  
b) ⌊v * 8⌋ = y  
c) (u , v) = (0.375, 0.25)  
⌊0.375 * 8⌋ = 3  
⌊0.25 * 8⌋ = 2  
(x, y) = (3, 2) = [Black]

<img src="images/lab4demo.gif" width="400">
