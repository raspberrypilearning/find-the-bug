## Upgrade your game

If you have time, you can add more levels and more distractions to your game. You could also change the sprite that is hiding. 

Here are the blocks you will need to hide the bug on a new level:

<code class="blocks" style="background-color: white">when backdrop switches to [new level v]</code><code class="blocks" style="background-color:white">set size to [20] %</code><code class="blocks" style="background-color:white">go to x: [0] y: [0] // drag to position the bug first</code><code class="blocks" style="background-color:white">set [color v] effect to [50]</code>

--- task ---
For each level you will need to:
- Add a backdrop
- Click on the Stage pane. Drag the new backdrop into position before the end backdrop. 
- Add a `when backdrop switches to`{:class="block3events"} block for the new backdrop and add code to position and hide the bug 

**Tip:** To drag the bug to a new hiding position you will need to 'break' the code so the bug doesn't switch to the backdrop when you are making a new level.

--- /task ---

--- task ---
You could add more parrots or choose another sprite to act as a distraction. 

Here is the code you used to for the parrot:
```blocks3
when flag clicked
set rotation style [left-right v] // don't go upside down
point in direction [35] // number from -180 to 180
forever // keep being annoying
move [10] steps // number controls speed
if on edge, bounce // stay on the Stage
next costume // flap
change [colour v] effect by [5] // try 11 or 50
wait [0.25] secs // try 0.1 or 0.5
end
```

**Tip:** You can drag the parrot's code to another sprite to make it faster to create another distraction sprite.

![Dragging code to another sprite](images/drag-parrot-code.png)

--- /task ---

--- save ---

<script>
scratchblocks.renderMatching("code.blocks", {
  inline: true,
  style:     'scratch3',   // Optional, defaults to 'scratch2'.
  // Repeat `style` and `languages` options here.
});
</script>
