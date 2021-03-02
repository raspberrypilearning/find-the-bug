## Add a first level

You will add a new backdrop as the first level in your game and hide the bug. 

--- task ---
Add the 'Spotlight' backdrop from the Music category.

--- /task ---

--- task ---

Click on the bug in the Sprite list. Add code to position your bug in the hiding place when the backdrop changes to Spotlight:

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
**Test:** Click the green flag to test your project. Click on the bug on the start screen and then click on the hidden bug on the Spotlight backdrop.

When you find the bug the project will go back to the Start screen. You'll add more levels to your game later.

--- /task ---

When you find the bug the project will go back to the start screen but the bug will still have the settings for the Spotlight backdrop. 

If you try and position the bug on the start screen it will switch to the next backdrop! That's not helpful when you are trying to position the bug.

--- task ---
Select the bug and drag the blocks away from the `when this sprite clicked` block to stop them running when you click on the bug:

![Breaking script to stop changes as you edit](breaking-script.gif)

--- /task ---

--- task ---

Drag the bug onto the Chalkboard on the Stage:

![Bug sprite positioned on the Chalkboard](images/bug-chalkboard.png)

--- /task ---

--- task ---

Add code to the bug to position on the Chalkboard every time your project switches to the Start screen:

![Bug sprite](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
go to x: [0] y: [30] // on the board
set size to [100] % // full size
```
--- /task ---

--- task ---
Join the blocks back to the `when this sprite clicked` block so that clicking the bug switches to the next backdrop:

![Code blocks joined back together](fixed-script.gif)

--- /task ---

--- task ---

**Test:** Click the green flag to test your project. 

--- /task ---

-- save ---