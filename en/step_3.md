## Add a first level

You will add a new backdrop as the first level in your game and hide the bug. 

--- task ---
Add the 'Spotlight' backdrop from the Music category.

--- task ---

--- task ---

Click on the bug in the Sprite list. Add code to hide your bug when the backdrop changes to Spotlight:

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
go to x: [13] y: [132] // on the disco ball
```

You can choose a different size and location if you prefer. 

--- /task --

When you successfully find the bug the game will switch to the next backdrop. You'll also start the game by clicking on the bug on the Start screen.

--- task ---

Add code to your bug to play a pop sound and switch to the next backdrop when you click on it:

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

Your project needs to start on the Start screen.

--- task ---

<mark>Should this be on the bug or the Stage?</mark>

```blocks3
when flag clicked
switch backdrop to [start v] // start screen
```

--- /task ---

--- task ---
Click the green flag to test your project. Click on the bug on the start screen and then click on the hidden bug on the Spotlight backdrop.

--- /task ---

