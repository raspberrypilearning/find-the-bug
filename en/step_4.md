## Add a parrot distraction

An annoying parrot distraction will make it harder for players to find and click on the bug. 

--- task ---
Add the parrot sprite. 

--- /task ---

A `forever`{:class="block3control"} loop runs the code blocks inside it over and over. It's perfect for an annoying parrot that just won't stop flying around and getting in the way.

--- task ---

Add code to make the parrot flap around in a distracting way:

![Parrot sprite](images/parrot-sprite.png)


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

--- /task ---

--- task ---
**Test:** Click the green flag and test your project again. Can you remember where you hid the bug? 

--- /task ---

--- save ---