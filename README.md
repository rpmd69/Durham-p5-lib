# Documentation
## boards.js
### Description
* A class that creates ten 'boards' in a given position. The boards are layered on top of each other when the mouse is directly on top of them and extend towards the mouse 
as the mouse moves around the sketch. The boards also perform a small animation where they individually move up and down one after the other. The height of this animation is changed 
depending on the x-coordinate of the mouse (the further away from the x-coordinate of the middle 'board', the larger the animation). 
### Fields and Methods
* **Constructor()**: 
	* **xPosition**: The x-coordinate of the middle rectangle of the sketch. 
	* **yPosition**: The y-coordinate of the middle rectangle of the sketch. 
	* **rectX**: The width of the rectangles. 
	* **rectY**: The height of the rectangles. 
	* **depth**: The thickness of the borders of the rectangles. 
	* **colour**: The colour of the rectangles. 
* **setXPosition(xPosition)**: Takes a given 'xPosition' and moves the sketch across the x axis accordingly. 
* **getXPosition()**: Gets the value of 'xPosition'.  
* **setYPosition(yPosition)**: Takes a given 'yPosition' and moves the sketch across the y axis accordingly. 
* **getYPosition()**: Gets the value of 'yPosition'. 
* **setRectX(rectX)**: Takes a given 'rectX' and extends the width of the rectangles accordingly. 
* **getRectX()**: Gets the value of 'rectX'. 
* **setRectY(rectY)**: Takes a given 'rectY' and extends the height of the rectangles accordingly. 
* **getRectY()**: Gets the value of 'rectY'. 
* **setDepth(depth)**: Takes a given 'depth' and changes the thickness of the border of the rectangles accordingly. 
* **getDepth()**: Gets the value of 'depth'.  
* **setColour(colour)**: Takes a given 'colour' (which is a hexadecimal value) and changes the colour of the rectangles accordingly. 
* **getColour()**: Gets the value of 'colour'. 
* **draw()**: 
	* **num**: The number of rectangles in the sketch. 
	* **intervalX**: Changes the height of the animation of the rectangles based on 'mouseX'. 
	* **intervalY**: Changes the height of the animation of the rectangles based on 'mouseY'. 
	* **tilt**: Calculates the coordinates of the corners of the rectangles based on the 'yPosition', 'xPosition', 'mouseX', and 'mouseY'. 
	* **rythm**: Calculates the position of each rectangle based on 'frameCount', 'mouseX', and 'xPosition'. 