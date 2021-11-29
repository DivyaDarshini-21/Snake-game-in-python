# Snake-game-in-python

T he sub-bits that build the Snake Game in Python:

1) Installing Pygame
2) Create the Screen
3) Create the Snake
4)  Moving the Snake
5) Game Over when Snake hits the boundaries
6) Adding the Food
7) Increasing the Length of the Snake
8) Displaying the Score


Installing Pygame:

The first thing you will need to do in order to create games using Pygame is to install it on your systems. To do that, you can simply use the following command:

pip install pygame

Once that is done, just import Pygame and start off with your game development. 


Create the Screen:

To create the screen using Pygame, you will need to make use of the display.set_mode() function. 
Also, you will have to make use of the init()  and the quit() methods to initialize and uninitialize everything at the start and the end of the code. 
The update() method is used to update any changes made to the screen. 
There is another method i.e flip() that works similarly to the update() function. 
The difference is that the update() method updates only the changes that are made (however, if no parameters are passed, updates the complete screen) but the flip() method redoes the complete screen again.

The next part is to draw our snake on the screen 

Create the Snake:
To create the snake, I will first initialize a few color variables in order to color the snake, food, screen, etc. 
The color scheme used in Pygame is RGB i.e “Red Green Blue”. In case you set all these to 0’s, the color will be black and all 255’s will be white. 
So our snake will actually be a rectangle. 
To draw rectangles in Pygame, you can make use of a function called draw.rect() which will help yo draw the rectangle with the desired color and size.


The next step is to get your snake moving.

Moving the Snake:

To move the snake, you will need to use the key events present in the KEYDOWN class of Pygame. 
The events that are used over here are, K_UP, K_DOWN, K_LEFT, and K_RIGHT to make the snake move up, down, left and right respectively. 
Also, the display screen is changed from the default black to white using the fill() method.
I have created new variables x1_change and y1_change in order to hold the updating values of the x and y coordinates.


Game Over when Snake hits the boundaries:

In this snake game, if the player hits the boundaries of the screen, then he loses. 
To specify that, I have made use of an ‘if’ statement that defines the limits for the x and y coordinates of the snake to be less than or equal to that of the screen. 
Also, make a not over here that I have removed the hardcodes and used variables instead so that it becomes easy in case you want to make any changes to the game later on.


Adding the Food:
Here, I will be adding some food for the snake and when the snake crosses over that food, I will have a message saying “Yummy!!”. 
Also, I will be making a small change wherein I will include the options to quit the game or to play again when the player loses.

Increasing the Length of the Snake:

 If the snake collides with his own body, the game is over and you ill see a message as “You Lost! Press Q-Quit or C-Play Again“. T
 he length of the snake is basically contained in a list 
 
 Displaying the Score:
 
Last but definitely not the least, you will need to display the score of the player. 
To do this, I have created a new function as “Your_score”. 
This function will display the length of the snake subtracted by 1 because that is the initial size of the snake.







