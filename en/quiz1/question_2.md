--- question ---

---
legend: Question 2 of 3
---

You used a `forever`{:class="block3control"} loop to make the parrot sprite fly around in an annoying way. 

We've tried to add another distraction sprite but it just moves once and then stops. How can we fix it?

![Rocket sprite](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [all around v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [colour v] effect by [25] 
wait [0.5] secs 
end
```

--- choices ---

- ( ) Change the number in the `wait`{:class="block3control"} block

  --- feedback ---
Changing the numbers in the `wait`{:class="block3control"} block will change how far the sprite moves when it is clicked but will not make the Rocketship keep moving.
  --- /feedback ---

- ( ) Remove the `if on edge, bounce`{:class="block3motion"} block.

  --- feedback ---
The `if on edge, bounce`{:class="block3motion"} block makes the sprite bounce off the edge of the Stage. If you removed it then the Rocketship would get stuck at the edge of the Stage.
  --- /feedback ---

- ( ) Add another`forever`{:class="block3control"} block.

--- feedback ---
A script can only have one forever block. Did you notice that you can't add a block underneath a `forever`{:class="block3control"} block?
--- /feedback ---

- (x) Drag the `move`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop.

  --- feedback ---
  Yes! The sprite only moves once. Moving the `move`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop will make it keep moving until you stop your project.
  --- /feedback ---

--- /choices ---

--- /question ---