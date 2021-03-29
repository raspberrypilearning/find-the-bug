## First level

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
You will add a new backdrop as the first level in your game and hide the bug.
</div>
<div>
![The Spotlight backdrop with a bug.](images/first-level.png){:width="300px"}
</div>
</div>

--- task ---

Add the **Spotlight** backdrop from the **Music** category.

![](images/backdrop-button.png)

--- /task ---

--- task ---

Click on the **bug** sprite in the Sprite list. Add a script to change the `size`{:class="block3looks"} of your bug `when the backdrop switches to Spotlight`{:class="block3events"}:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
``` 

--- /task ---

--- task ---

Click on the code to change the size, then drag your tiny bug to a hiding place. 

Add code to position your bug:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Choose:** You can choose a different size and location, if you prefer. 

--- /task ---

When you play the game and you successfully find the bug, the game will switch to the next backdrop. Also, to start the game, you will click on the bug on the 'start' screen.

The `next backdrop`{:class="block3looks"} block switches to the next backdrop in the order in which the backdrops are listed when you click on the Stage pane. 

--- task ---

Add a script to your **bug** sprite to `play a pop sound`{:class="block3sound"} and switch to the `next backdrop`{:class="block3looks"} `when this sprite is clicked`{:class="block3events"}:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

Your project needs to start on the 'start' screen.

--- task ---

Click on the Stage pane and add this code to the **Stage**:

![Image of the Stage icon.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // start screen
```

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. 

You will notice that on the 'start' screen, the bug will still have the settings to hide on the disco ball on the first level. 

**Tip:** After the last backdrop in the list, `next backdrop`{:class="block3looks"} will switch back to the first backdrop.

--- /task ---

--- task ---

Click on the **bug** sprite. Add a script to `set the size`{:class="block3looks"} of the bug when your project `switches to the start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full size
```

--- /task ---

--- task ---

Try to position the bug on the 'start' screen. 

Your code will make it switch to the next backdrop! That is not helpful when you are trying to position the bug.

--- /task ---

To fix the problem, you need to stop the code from running when you click on the bug.

--- task ---
Click on the green flag to return to the 'start' screen.

Click on the **bug** sprite and drag the blocks away from the `when this sprite clicked`{:class="block3events"} block:

![Breaking the script to stop changes as you edit.](images/breaking-script.png)

--- /task ---

--- task ---

Try to position the bug again. Drag the bug onto the chalkboard, below the text: 

![](images/bug-chalkboard.png)

Add code to make sure that the bug is positioned on the chalkboard every time your project switches backdrop to the 'start' screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

Join the blocks back together so that the code blocks are under the `when this sprite clicked`{:class="block3events"} block.

![](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. Click on the bug to move to the next backdrop. The bug should be big on the 'start' screen and small on the 'Spotlight' level.

--- collapse ---

---
title: Nothing happens when I click on the bug
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---

--- save ---
