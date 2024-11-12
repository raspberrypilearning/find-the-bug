--- question ---
---
legend: Question 2 of 3
---

You used a `forever`{:class="block3control"} loop to make the **Parrot** sprite fly around in an annoying way.

We have tried to add another distraction sprite, but it just moves once when we click on the green flag and then stops. How can we fix it?

![The Rocket sprite.](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [all around v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [color v] effect by [25] 
wait [0.5] seconds 
end
```

--- choices ---

- ( ) Change the number in the `move`{:class="block3motion"} block

  --- feedback ---

If you change the number in the `move`{:class="block3motion"} block, you will change how far the sprite moves when the green flag is clicked, but this change will not make the rocket keep moving.

  --- /feedback ---

- ( ) Remove the `if on edge, bounce`{:class="block3motion"} block

  --- feedback ---

The `if on edge, bounce`{:class="block3motion"} block makes the sprite bounce off the edge of the Stage. If you removed it, then the rocket would get stuck at the edge of the Stage.

  --- /feedback ---

- ( ) Add another `forever`{:class="block3control"} block

--- feedback ---

A script can only have one `forever`{:class="block3control"} block. Did you notice that you cannot add a block underneath a `forever`{:class="block3control"} block?

--- /feedback ---

- (x) Drag the `move`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop

  --- feedback ---

  Da! The sprite only moves once. If you move the `move`{:class="block3motion"} block inside the `forever`{:class="block3control"} loop, the sprite will keep moving until you stop your project.

  --- /feedback ---

--- /choices ---

--- /question ---
