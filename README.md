# 2520-Assignment6
# Assignment 6 Read me [2520.02]
##graphics_v4.py

Code Documentation:

Program Objective lines:
	Make the program easy to adapt to other programs and for modularity and modify the code in a way that allows for easy modifications such as altering object locations, quantities, and sizes.

Modification to clouds (lines 51-86):
	Added a function draw_cloud(x, y) to encapsulate the drawing logic for the cloud, which takes in the cloud's coordinates (x, y) as input parameters.
Moved the cloud drawing logic from the main game loop to the draw_cloud() function, and replaced the previously hard-coded color values with the cloud_color variable that is determined based on the day variable. Allowed for simplier code and the same purpose

Refresh rate (line 19) : 
	Allowed the user to choose the refresh rate based on the spped level that they type in 

Lights-on(line 92-103):
	Allowed the user to use a True or False value for lights 
	Added two boolean variables, day and lights_on, to represent the current state of the day/night cycle and lights status respectively.
Wrapped the event processing logic inside a for loop that iterates over all events in the event queue using pygame.event.get().
Added event handling for two keys: 'l' to toggle the lights on/off, and 'd' to toggle between day and night mode.
Modified the game logic to use the day and lights_on variables to determine the appropriate colors for the sky, field, stripe, cloud, and fence based on the current state of light.

Number of stars and clouds:
	This code generates a random number of stars and clouds based on user input for "little", "middle", or "alot". If the user input is not recognized, it defaults to a certain number. The code then creates lists to store the coordinates and size of the stars, and the coordinates of the clouds, using the random module to generate random numbers within certain ranges. Finally, the function returns these lists.


Members:
Natalia Jauregui
