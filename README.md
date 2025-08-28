.Created Two Files
->index.html
->app.js

=>HTML
.Added Phaser library and javascript files to the header file in html

=>JS
.Created three main functions of my game 
1.preload-to bring background for the game
2.create - to generate the background of the game
3.update - to update the position of the bird

.Creating a game variable of a new instance of Phaser.Game to set up the game. I pass in the config object and specify these parameters about the game we want to create:
1.The width and height of the game screen (800 x 600 pixels).
2.The physics system of our game; we're using 'arcade'.
3.A scene object with the functions we want to use in it, including preload(), create(), and update().

.Created preload() function - I am loading in the images from my assets folder. For the bird image, we load it as a 'sprite', not an image. In Phaser, a 'sprite' can be animated.
.Created create() function - With the setOrigin() method, we specify that we want the upper left corner of the background to be positioned at (0, 0).
For our clone application, we're just going to place a single road at the bottom of the game screen. While it won't move like it does in the actual game.
When we write this.physics, we are making a call to the Arcade Physics system in Phaser. This will allow us to apply a physics simulation to the roads we create.

The roads variable allows us to create a single, static road variable.

We specify that we want "roads" to have a static body.

With the setScale() method, we specify that we want the road to be twice as big as its original size. Since we changed the size, we need to add a call to the refreshBody() method in order for the physics to work now that the size has changed.
