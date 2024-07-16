This Portfolio was created by Lara Remmelberger and Marlon Schiedeck.



Technology used for this project:

(html, p5.js)

In order to be able to display the portfolio like a website, we decided to work with html and p5.js, which is an open source library for java script that resembles processing (a programming language mainly used for creating visual art).



Algorithm: 
1. Layers:
   Our code uses layers to implement a specific kind of visual effect. Some of those layers look like a regular main canvas with a background and others are more like a png with a transparent background.
   
3. Rectangles:
   In the beginning the user can create 5 rectangles. When you click your left mouse and move it you will open a rectangle that shifts its size and form according to where you drag the cursor. Only once you release the mouse, the rectangle will be finalizes.
   Instead of drawing a rectangle on the canvas though, you're actually cutting thorugh the first (black) layer and the 2nd (blue) layer underneath is revealed.
   During this process the code will check, wether the rectangle you're creating overlaps with any already existing rectangle. If it does, the overlapping part will cut through the 2nd layer as well, revealing the 3rd (red) layer and thus look red.
   
5. Tree:
   The user can plant a tree with a mouse click. From that postion it will grow on a layer with a transparent background on top of all the other layers using ellipses. Regularly the tree will be covered by a colorful shading to make the tree appear 3d,
   but when it's growing inside of a cut out rectangle the tree will loose its shade and appear 2d. This is achieved by checking for overlapping parts and drawing small colorfull elleipses on top of the big white ellipses.
   
7. Fractal structures:
   The drawFractal functions are responsible for drawing fractal patterns on the respective graphics layers, so that they appear in the background. These fractals are created using a recursive approach,
   where each function calls itself to draw smaller segments of the fractal. The fractal is divided into n segments a loop runs n times to create n segments. This creates complex patterns by dividing each segment into smaller segments,
   and n controls the number of segments at each level of recursion, thus affecting the complexity and appearance of the fractal



End result: 

Our end result is a website with a canvas which can be used to create endless amounts of outputs of a collage like artpiece. 
Those eldless amounts of different artpieces are achieved by a certain degree of randomness in our code, but mostly by user interactivity.
The users can draw rectangles in different sizes and positions, plant a flexible amount of trees on the canvas and change the background structure by putting in numbers on the top left of the canvas. Ultimately the user can try out different compositions and structures and generate an infinite amount of different art pieces.
We have combined mathematical geometric structures with organic ones which contrast in bright neon colors. 
Red and blue rectangles are drawn on the canvas and trees with a colorful shading can be planted.
