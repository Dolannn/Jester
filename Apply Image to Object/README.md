# Jester SQF Tuts\Apply Image to Object
Author: Dolan

Firstly, pick an image, make sure the dimensions of the image are one of the following (the dimensions of am image can be modified via a program / websites like photoshop, https://www.photopea.com/, paint etc etc

*** Valid Image Dimensions ***

NOTE: You can combine dimensions like 512x256 also

64x64

256x256

512x512

1024x1024

2048 x 2048

*YOUR IMAGE MUST BE SAVED AS EITHER A .paa OR a .jpg!*

Launch your mission in the ARMA Editor. In the top left of your screen, click "Scenario > Open Scenario Folder"

Your mission directory will open, right click and hover over "New > Folder" name this folder "images" (make sure it has a lowercase "i")

Place your image into this folder. Keep track of what you named it, for this example my image is called "myPhoto1"

Alt-Tab back into Arma 3, hit Ctrl + S to save your mission, this allows Arma to see what changes you just did.

Place down an object like a billboard, a sign, a laptop etc, double click on it once it's placed.

In the Object: Init box put the following piece of code in:


this setObjectTextureGlobal [0,"images\myPhoto1.jpg"];


Remember if you're using a different name lets say named it "jesterPhoto.jpg", replace \myPhoto1.jpg in the code to \jesterPhoto.jpg

Save yor mission and see if it worked!
