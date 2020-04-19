# Lab 3 for CMPM 163
Introduction to THREE.js Materials and Shaders.

Google Drive link to video:
https://drive.google.com/open?id=1Shr7l23jnsXnxEopUK96pCQb2x88-GGr

## Writeup

Top Left: On top of having the color changed to a bronze brown and the specular to a cobalt blue, the material was also given a weak emissive white color, as demonstrated by a lack of a dark side compared to its right counterpart. It also has a very light transparency with the opacity set to 0.75, however this is less noticeable.

Top Right: Followed baseline instructions of Part 1.

Bottom Left: Followed baseline instructions of Part 2.

Bottom Right: For starters, the colors for interpolation were tweaked to use pale white and orange colors. However, as can be seen, that's not where it ends; in the fragmentShader component of this cube, the colorZ component is warped not just by a single vertex, but instead by the Y component divided by Z. This results in the strange jarring of the two colors at weird places such as the center of certain edges of the cube due to the mathematic outcomes of this simple division using irrelevant inputs.

<img src="images/lab3demo.gif" width="400">
