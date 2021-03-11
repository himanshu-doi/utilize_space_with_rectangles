# utilize_space_with_rectangles
Fill rectangles to utilize all available space in an outer rectangle with two pre-existing inner rectangles  

## Problem
Here input is the height and width of the outer and inner rectangles along with their left bottom x,y coordinates.
The origin can be assumed to be at the left bottom coordinate of the outer rectangle.
We need to draw more rectangles so that all the space inside the outer rectangle is utilized.

## Solution
I calculate the left bottom and right top coordinates of the two inner rectangles and use them to pack all available space inside.
Firstly, outer boundary rectangles are made if they satisfy the minimum rectangle side length. Post that inner rectangles are packed based on their orientation.
The solution also has a "pad" variable to space all rectangles evenly. Default padding is set to 5 pixels.

Output of the "draw_all_rectangles" method is the left bottom coordinate(x, y), width and height of the newly drawn rectangles.

