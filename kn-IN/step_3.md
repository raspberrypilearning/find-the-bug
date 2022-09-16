## ಮೊದಲ ಹಂತ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![The Spotlight backdrop with a bug.](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

**Music** ವರ್ಗದಿಂದ **Spotlight** ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಸೇರಿಸಿ.

!['Choose a Backdrop' ಐಕಾನ್.](images/backdrop-button.png)

--- /task ---

### Resize the bug

--- task ---

ಸ್ಪ್ರೈಟ್ ಪಟ್ಟಿಯಲ್ಲಿರುವ **bug** ಸ್ಪ್ರೈಟ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. `when the backdrop switches to Spotlight`{:class="block3events"} ಆದಾಗ ನಿಮ್ಮ ದೋಷದ `size`{:class="block3looks"} ಬದಲಾಯಿಸಲು ಬರಹ ಸೇರಿಸಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

ಗಾತ್ರವನ್ನು ಬದಲಾಯಿಸಲು ಕೋಡ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ, ನಂತರ ನಿಮ್ಮ ಸಣ್ಣ ದೋಷವನ್ನು ಅಡಗುದಾಣಕ್ಕೆ ಎಳೆಯಿರಿ.

ನಿಮ್ಮ ದೋಷವನ್ನು ಇರಿಸಲು ಕೋಡ್ ಸೇರಿಸಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Choose:** ನೀವು ಬಯಸಿದಲ್ಲಿ ಬೇರೆ ಗಾತ್ರ ಮತ್ತು ಸ್ಥಳವನ್ನು ಆಯ್ಕೆ ಮಾಡಬಹುದು.

--- /task ---

### Move to the next Backdrop

ನೀವು ಆಟವನ್ನು ಆಡುವಾಗ ಮತ್ತು ದೋಷವನ್ನು ಯಶಸ್ವಿಯಾಗಿ ಕಂಡುಕೊಂಡಾಗ, ಆಟವು ಮುಂದಿನ ಹಿನ್ನೆಲೆಗೆ ಬದಲಾಗುತ್ತದೆ. ಅಲ್ಲದೆ, ಆಟವನ್ನು ಪ್ರಾರಂಭಿಸಲು, ನೀವು 'start' ' ಪರದೆಯ ಮೇಲೆ ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡುತ್ತೀರಿ.

`next backdrop`{:class="block3looks"} ಬ್ಲಾಕ್ ನೀವು **Stage**ನ **Backdrops** ಟ್ಯಾಬ್ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿದಾಗ ಬ್ಯಾಕ್ಡ್ರಾಪ್‌ಗಳು ಪಟ್ಟಿಯಾದ ಕ್ರಮದಲ್ಲಿ ನಂತರ ಬರುವ ಬ್ಯಾಕ್ಡ್ರಾಪ್‌ಗೆ ಬದಲಾಗುವುದು.

--- task ---

`play a Pop sound`{:class="block3sound"} ಮಾಡಲು ಮತ್ತು `next backdrop`{:class="block3looks"} `when this sprite is clicked`{:class="block3events"}ಬದಲಾಯಿಸಲು ನಿಮ್ಮ **bug** ಸ್ಪ್ರೈಟ್ ಗೆ ಬರಹ ಸೇರಿಸಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

### Make the game start with the Start Screen

--- task ---

Click on the Stage pane and add this code to the **Stage**:

![The Spotlight backdrop.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // 'start' screen
```

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project.

You will notice that on the 'start' screen, the bug will still have the settings to hide in its hiding place from the first level (in this example, on the disco ball).

**Tip:** After the last backdrop in the list, `next backdrop`{:class="block3looks"} will switch back to the first backdrop.

--- /task ---

--- task ---

Click on the **bug** sprite in the Sprite list. Add a script to `set the size`{:class="block3looks"} of the bug when your `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
```

--- /task ---

### Change the position of the bug

--- task ---

Try to position the bug on the 'start' screen.

Your code will make the backdrop switch when you click on the bug! That is not helpful when you are trying to position the bug.

To fix the problem, you need to stop the code from running when you click on the bug.

--- /task ---

--- task ---

Click on the green flag to return to the 'start' screen.

Click on the **bug** sprite in the Sprite list and drag the blocks away from the `when this sprite clicked`{:class="block3events"} block:

![Breaking the script.](images/breaking-script.png)

--- /task ---

--- task ---

Try to position the bug again. Drag the bug onto the chalkboard, below the text:

![The bug on the start screen](images/bug-chalkboard.png)

Add code to make sure that the bug is positioned on the chalkboard every time your `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

Join the blocks back together so that the code blocks are under the `when this sprite clicked`{:class="block3events"} block again:

![The 'when this sprite clicked' block joined to the 'play sound' and 'next backdrop' blocks.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. Click on the bug to move to the next backdrop. The bug should be big on the 'start' screen and small on the 'Spotlight' level.

--- collapse ---
---
title: ನಾನು ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಏನೂ ಆಗುವುದಿಲ್ಲ
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---