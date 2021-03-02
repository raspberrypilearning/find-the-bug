--- question ---

---
legend: Question 3 of 3
---

Oh no! You dragged the bug into a new position and now the bug is on top of the parrot. 

![Stage with bug on top of parrot](images/bug-reorder.png)

What can you do to the bug sprite to fix this and make sure this doesn't happen again? 

![Bug sprite](images/bug-sprite.png)

--- choices ---

- ( ) On the Stage, drag the parrot on top of the bug.

  --- feedback ---
This will fix the problem once. But, dragging the bug on the Stage will send it back to the front again.
  --- /feedback ---

- ( ) Click on the `go to [] layer`{:class="block3looks"} block in the `Looks`{:class="block3looks"} Blocks menu.

  --- feedback ---
If you click on `go to [back v] layer`{:class="block3looks"} when you have the bug selected then this will fix the problem once. But, dragging the bug on the Stage will send it back to the front again.
  --- /feedback ---

- (x) Add a `go to [back v]`{:class="block3looks"} layer in a `forever`{:class="block3lcontrol"} loop to the bug. 

  --- feedback ---
Yes, adding a `go to [back v]`{:class="block3looks"} layer in a `forever`{:class="block3control"} loop will make the bug always appear at the back:

```blocks3
when flag clicked
forever
go to [back v] layer
```
  --- /feedback ---

- ( ) Add a `go to [front v]`{:class="block3looks"} layer in a `forever`{:class="block3control"} loop to the bug. 

  --- feedback ---

This will make the bug go to the front, not the back.

  --- /feedback ---

--- /choices ---

--- /question ---