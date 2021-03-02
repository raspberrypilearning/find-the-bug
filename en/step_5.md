## Add a second level

You will choose a backdrop and hide your bug to make a second level for your game. 

--- task ---

Choose a backdrop to hide your bug in. We have chosen **Urban** but you can choose the one you like best. 

![inserted Urban backdrop](images/insert-urban-backdrop.png)

**Tip:** Remember that backdrops with lots of colours and details will make the bug harder to find. How difficult will you make your game?  

--- /task ---

You will position your bug and change the size so that it is hidden in this new level.

--- task ---

Drag the blocks away from the `when this sprite clicked`{:class="block3events"} block to stop them running when you click on the bug:

![Breaking script to stop changes as you edit](breaking-script.gif)

--- /task ---

--- task ---

Add code to resize the bug when the backdrop switches to the Urban backdrop:

![Bug sprite](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
```

--- /task ---

--- task ---

Click on your new code to run it then drag your bug on the Stage to a good hiding place for this level. 

![bug hidden on Urban backdrop](images/hidden-urban-backdrop.png)

--- /task ---

--- task ---

Add code to position your bug in the hiding place when the backdrop changes to your chosen backdrop:

![Bug sprite](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

--- task ---
Join the blocks back to the `when this sprite clicked`{:class="block3events"} block so that clicking the bug switches to the next backdrop:

![Code blocks joined back together](fixed-script.gif)

--- /task ---

--- task ---

**Test:** Click the green flag to test your project. 

--- /task ---

Your bug may now be in front of the parrot. 

--- task ---

Add a script to make sure your bug is always at the back:

![Bug sprite](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Now your bug will always stay at the back even if you need to reposition it.

--- /task ---

--- save ---