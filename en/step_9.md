## Upgrade your game

If you have time, you can add more levels and more distractions to your game. You could also change the sprite that is hiding and change the text on the chalkboard. 

--- task ---

Play your game and see how quickly you can find the bugs. 

Is there someone else who can try your game? How fast can they find the bugs? They will not know where you have hidden them, so it might take them a bit longer!

Is there anything that you want to change?

You could:
- Make the parrot even more annoying
- Make the bugs smaller 
- Change the `color effect`{:class="block3looks"} to camouflage the bug on each level
- Change the font or colour of the text

--- /task ---

### Add more levels

--- task ---

Here are the blocks that you will need to hide the bug on a new level:

```blocks3
when backdrop switches to [new level v]

set size to [20] %

go to x: [0] y: [0] // drag to position the bug first

set [color v] effect to [50]
```

For each level, you will need to:
- Add a backdrop
- Click on the Stage pane, then on the **Backdrops** tab, then drag the new backdrop into position before the **end** backdrop
- Add a `when backdrop switches to`{:class="block3events"} block for the new backdrop and add code to position and hide the bug 

**Tip:** To drag the bug to a new hiding position, you will need to 'break' the code so that the backdrop does not switch when you click on the bug to position it for a new level.

--- /task ---

### Add more distractions

--- task ---

You could add more parrots or choose another sprite to act as a distraction. 

Here is the code that you used for the parrot:

```blocks3
when flag clicked
set rotation style [left-right v] // do not go upside down
point in direction [35] // number from -180 to 180
forever // keep being annoying
move [10] steps // the number controls the speed
if on edge, bounce // stay on the Stage
next costume // flap
change [color v] effect by [5] // try 11 or 50
wait [0.25] seconds // try 0.1 or 0.5
end
```

**Tip:** You can drag the **Parrot** sprite's code to another sprite to make it faster to create another distraction sprite.

![Dragging code from the Code area to another sprite in the Sprite list.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Completed project
---

You can view the [completed project here](https://scratch.mit.edu/projects/486719939/){:target="_blank"}.

--- /collapse ---

### Community submissions

--- task ---

Inspire the Raspberry Pi Foundation community with your project! 

[[[share-scratch]]]

To submit your project to our 'Find the bug' Scratch studio for other people to see, please complete [this form](https://form.raspberrypi.org/f/community-project-submissions){:target="_blank"}.

--- /task ---

--- no-print ---
--- task --- 

Play these fabulous games from our 'Find the bug' Scratch studio [See inside](https://scratch.mit.edu/studios/29005236/){:target="_blank"}.

Notice how the creators have added extra levels, annoying distractions or upgraded the start and end screens:

<div class="scratch-preview" style="margin-left: 15px;">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/545488112/?autostart=false" frameborder="0"></iframe>
</div>

<div class="scratch-preview" style="margin-left: 15px;">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/707645119/?autostart=false" frameborder="0"></iframe>
</div>

<div class="scratch-preview" style="margin-left: 15px;">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/707644397/?autostart=false" frameborder="0"></iframe>
</div>

--- /task ---

--- /no-print ---

--- task ---

You can also look at the remixes for the [Find the bug starter project](https://scratch.mit.edu/projects/582214723/remixes){:target="_blank"} to see what other creators have made.

--- /task ---

--- save ---

