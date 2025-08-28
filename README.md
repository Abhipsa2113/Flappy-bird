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
