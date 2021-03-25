## Second level

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
You will choose a backdrop to make a second level for your game and make the bug hard to find. 
</div>
<div>
![Street scene with hidden bug.](images/second-level.png){:width="300px"}
</div>
</div>

--- task ---

**Choose:** Choose a backdrop for your second level. We have chosen the **Urban** backdrop, but you can choose the one that you like the most. 

![](images/insert-urban-backdrop.png)

**Tip:** Remember that backdrops with lots of colours and details will make the bug harder to find. How difficult will you make your game?  

--- /task ---

To be able to drag your bug into a new position, you need to stop the `when this sprite clicked`{:class="block3events"} code from running.

--- task ---

Drag the blocks away from the `when this sprite clicked`{:class="block3events"} block to stop them running when you click on the bug:

![](images/breaking-script.png)

--- /task ---

Your bug needs to be hard to find when the backdrop changes. You can resize the bug to make it harder to find.

--- task ---

Add code to resize the bug when the backdrop switches.

![Bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Test:** Click on your new script to run it.

--- /task ---

--- task ---

Drag your bug on the Stage to a good hiding place for this level. 

![Bug hidden in the window in the middle of the backdrop.](images/hidden-urban-backdrop.png)

--- /task ---

Position your bug in its hiding place.

--- task ---

Add a `go to x: y:`{:class="block3motion"} block to your code.

![Bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

--- task ---
Join the blocks back to the `when this sprite clicked`{:class="block3events"} block so that clicking on the bug switches to the next backdrop:

![](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. 

--- /task ---

Your bug may now be in front of the parrot. 

--- task ---

Add a script to make sure that your bug is always at the back:

![Bug sprite.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Now, your bug will always stay at the back, even if you need to reposition it.

--- /task ---

--- save ---
