## Add an end screen

Create an end screen to show the number of seconds it has taken to find the bugs. 

--- task ---

Add the 'Chalkboard' backdrop from the Indoors category. 

![A chalkboard on a wall](images/chalkboard.png)

**Tip:** In Scratch you can add the same backdrop more than once.

--- /task ---

Click on the 'Backdrops' tab to open the Paint editor. 

![Chalkboard backdrop in the Paint editor](images/chalkboard-paint.png)

--- /task ---

--- task ---

Change the name of the backdrop to 'end':

![Backdrop name changed to Start screen in the paint editor](images/end-screen-name.png)

--- /task ---

--- task ---
Add code to position the bug on the end screen:

![Bug sprite](images/bug-sprite)

```blocks3
when backdrop switches to [end v]
go to x: [0] y: [30] // on the board
set size to [100] % // full size
```

**Tip:** Renaming the backdrop to end makes it easier to understand your code. 

--- /task ---

How long does it take you to find and click on the bugs? Scratch has a built-in `timer`{:class="block3sensing"} that you can use to find out.

--- task ---

The `timer`{:class="block3sensing"} is in the `Sensing`{:class="block3sensing"} Blocks menu.

![Bug sprite](images/bug-sprite)

```blocks3
when backdrop switches to [end v]
go to x: [-75] y: [30] // on the board
set size to [100] % // full size
+say (timer) // seconds taken
```

--- /task ---

--- task ---

**Test:** Click the green flag to test your finding skills. How long does it take you to find a click on the bug?

--- /task ---

You can click on the bug on the end screen to go back to the start screen. 

--- task ---
Add code to make the bug stop saying the timer when you go to the start screen:

![Bug sprite](images/bug-sprite)

```blocks3
when backdrop switches to [start v]
go to x: [0] y: [30] // on the board
set size to [100] % // full size
+say [] // say nothing
```

--- /task ---

--- task ---

If you play the game a second time, the `timer`{:class="block3sensing"} will keep counting. 

--- /task ---

--- task ---

Reset the timer when you switch to the first level:

![Bug sprite](images/bug-sprite)

```blocks3
when backdrop switches to [Spotlight v]
+reset timer // start the timer
set size to [20] % // tiny
go to x: [13] y: [132] // on the disco ball
```

--- /task ---

--- task ---

**Test:** Click the green flag and play the game. The timer should reset when you click on the bug on the start screen to move to the first level. When you click on the bug on the end screen you should return to the start screen and see that the bug is not saying the timer. 

--- /task ---

--- save ---
