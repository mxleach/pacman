# Simple Pacman Exercise - Full Stack w/ MERN MIT/xPro

## Description
<br>
In this assignment we were given some starting code, but needed to make the fixed "Pacman" image on the screen 'chomp' his way back and forth upon reaching either side of the screen. The two main tasks in the assignment were: 

* Completing the Run() Function 
* Creating the checkPageBounds Functions

### Run() Function: 
This function is called on mouseclick. It grabs the image element by 'ID', and constantly updates the Pacman image, position and direction on the screen. The Run function allows the element to move across the screen, and does so by oscillating through an array pacArray, which contains two arrays inside - one for the focus and the other for direction. 

Each array within pacArray contains two images, the first contains Pacman's mouth open and closed going from left to right. The second contains Pacman's mouth open and closed going right to left. 

The run function grabs the element image, sets the image width, and calculates the function while limiting its result between 0 and 1, according to the Array. 

It then calls the checkPageBounds function, passing the intial direction (0), the image width, the current position (pos) and the pageWidth. Then we get the image source through the array of images by passing the direction we want the image to be on and the focus. 

As it iterates, we check to see if PacMan is moving forward. If true, we add 20px to its current position, and will move it 20px to the right. Otherwise, we subtract 20px, moving it to the left. 

Finally, setTimeout is called with the Run function with the parameter of 200ms. 



### checkPageBounds Function:
This function needs the diresction, imageWidth, pos, and pageWidth to work 
* direction: the current direction the images is moving to (0 or 1). 
* imageWidth: the width of the image in integer. 
* pos: the current position of the image in the document 
* pageWidth: the window inner width.

This function will change the Pacman's direction when it hits one of the edges. 


## Link to Pacman GitPage:
