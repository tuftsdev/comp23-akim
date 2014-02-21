By: Aromie Kim
CS login username: akim14
Dates: February 15-18, 2014


LAB 3: The Battle for Ram Aras, Part I 
Time taken: Roughly 5-7 hours
This lab involves the implementation of two sprites: a battlecruiser and a laser.


Name: Battlecruiser.py
This class utilizes the Laser class as a module, keeping a list of Lasers. The battlecruiser has a set of keyboard-based controls. These controls enable it to
move fluidly across the screen (fluid, continuous movement is enabled by key-holding)
and also enable it to shoot a laser once the spacebar is pressed.
The battlecruiser moves at a set speed (dx and dy are both a value of 4, so the position of the battlecruiser changes by 4).
The battlecruiser's image asset is defined within the class. There is a loading-image function that includes exception handling when the provided image does not exist or could not be found/open.
When Battlecruiser.py is run via the command "python Battlecruiser.py", a 800x600 window is produced with a screen containing the battlecruiser on a black background. The battlecruiser can then be
controlled via the proper controls:
     Move up = Up key
     Move down = Down key
     Move left = Left key
     Move right = Right key
     Fire laser = Spacebar
     Quit = Escape button
At the moment, the battlecruiser can move out of the screen. 


Name: Laser.py
This class is responsible for a laser sprite that moves vertically across the screen.
This sprite is not controllable by the user. 
The image to be loaded for this sprite is defined in the class. The loading-image function includes exception-handling.
The main creates a list of lasers of varying velocities. When Laser.py is run via the command "python Laser.py", a 800x600 window with a black screen will be made. A barrage of lasers will be
displayed traveling vertically up the screen at different speeds (speeds determined by "randint").
When this class is used as a module by the Battlecruiser, each laser bolt moves at a set speed (dx is 0 and dy is 10, so it changes y-position by 10). When shot out, the laser bolt moves out from the center of the battlecruiser. The laser bolt is deleted (killed) when it travels off the screen.
