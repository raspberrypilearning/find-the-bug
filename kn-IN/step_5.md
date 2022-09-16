## ಎರಡನೇ ಹಂತ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Choose a backdrop to make a second level for your game, and make the bug hard to find. 
</div>
<div>

! [ಗುಪ್ತ ದೋಷವಿರುವ ಬೀದಿ ದೃಶ್ಯ.](images/second-level.png){:width="300px"}

</div>
</div>

### Add another backdrop

--- task ---

**Choose:** ನಿಮ್ಮ ಎರಡನೇ ಹಂತಕ್ಕೆ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಆಯ್ಕೆಮಾಡಿ. **Urban** ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಅನ್ನು ಆಯ್ಕೆ ಮಾಡಿದ್ದೇವೆ, ಆದರೆ ನಿಮಗೆ ಹೆಚ್ಚು ಇಷ್ಟವಾದುದನ್ನು ನೀವು ಆಯ್ಕೆ ಮಾಡಬಹುದು.

![The bug and parrot on an urban backdrop.](images/insert-urban-backdrop.png)

**ಸಲಹೆ:** ಸಾಕಷ್ಟು ಬಣ್ಣಗಳು ಮತ್ತು ವಿವರಗಳನ್ನು ಹೊಂದಿರುವ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್‌ಗಳು ದೋಷವನ್ನು ಕಂಡುಹಿಡಿಯುವುದನ್ನು ಕಷ್ಟಕರವಾಗಿಸುತ್ತವೆ ಎಂಬುದನ್ನು ನೆನಪಿಡಿ. ನಿಮ್ಮ ಆಟವನ್ನು ನೀವು ಎಷ್ಟು ಕಷ್ಟಕರವಾಗಿಸುತ್ತೀರಿ?

--- /task ---

### Stop the code from running

--- task ---

Drag the blocks away from the `when this sprite clicked`{:class="block3events"} block to stop them from running when you click on the bug:

![Breaking the code.](images/breaking-script.png)

--- /task ---

### Resize the bug

--- task ---

Add code to `set the size`{:class="block3looks"} of the bug for the second level:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Test:** Click on your new script to run it.

--- /task ---

### Hide your bug

--- task ---

Drag your bug on the Stage to a good hiding place for this level.

![The bug hidden in the shop window in the middle of the backdrop.](images/hidden-urban-backdrop.png)

--- /task ---

Position your bug in its hiding place.

--- task ---

Add a `go to x: y:`{:class="block3motion"} block to your code:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

### Test your code

--- task ---

Join the blocks back to the `when this sprite clicked`{:class="block3events"} block so that when the bug is clicked, the backdrop switches to the `next backdrop`{:class="block3looks"}:

![The blocks are joined back together.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project.

--- /task ---

Your bug may now be in front of the parrot.

--- task ---

Add a script to make sure that your bug is always at the `back`{:class="block3looks"}:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Now, your bug will always stay at the back, even if you need to change its position.

--- /task ---
