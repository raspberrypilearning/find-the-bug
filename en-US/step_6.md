## End screen

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
You will create an 'end' screen to show the number of seconds that it has taken the player to find the bugs. 
</div>
<div>

![The bug with the amount of time in a speech bubble.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Sometimes, just beating a game isn't enough. Players like to know how they did against other players or themselves. Can you think of a game that shows you how well you did?</p>

--- task ---

Add the **Chalkboard** backdrop from the **Indoors** category.

![The Chalkboard backdrop in the Backdrop Library.](images/chalkboard.png)

**Tip:** In Scratch, you can add the same backdrop more than once.

--- /task ---

--- task ---

Click on the **Backdrops** tab to open the Paint editor.

![The Chalkboard backdrop in the Paint editor.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

Change the name of the backdrop to `end`:

![The backdrop name changed in the Paint editor.](images/end-screen-name.png)

**Tip:** You rename the backdrop to **end** to make it easier to understand your code.

--- /task ---

--- task ---

Click on the **bug** sprite and add code to position the bug on the 'end' screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
```

--- /task ---

How long does it take you to find and click on the bugs? Scratch has a `timer`{:class="block3sensing"} that you can use to find out.

--- task ---

The `timer`{:class="block3sensing"} block is in the `Sensing`{:class="block3sensing"} blocks menu. Add code to make the bug `say`{:class="block3looks"} the `timer`{:class="block3sensing"} on the 'end' screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say (timer) // seconds taken
```

![Inserting a 'timer' block into a 'say' block.](images/inserting-blocks.gif)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your finding skills. How long does it take you to find the bug?

--- /task ---

To go back to the 'start' screen, click on the bug on the 'end' screen.

--- task ---

Add code to make the bug stop saying the `timer`{:class="block3sensing"} when you go to the 'start' screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say [] // say nothing
```

--- /task ---

If you play the game a second time, the `timer`{:class="block3sensing"} will keep counting.

--- task ---

Add code to `reset the timer`{:class="block3sensing"} when the `backdrop switches to`{:class="block3events"} the first level:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // first level
set size to [20] % // tiny
go to x: [13] y: [132] // on the disco ball
+reset timer // start the timer
```

--- /task ---

--- task ---

**Test:** Click on the green flag and play the game. The timer should reset when you click on the bug on the 'start' screen to move to the first level. When you click on the bug on the 'end' screen, you should return to the 'start' screen and see that the bug is not saying the `timer`{:class="block3sensing"}.

--- /task ---

--- save ---
