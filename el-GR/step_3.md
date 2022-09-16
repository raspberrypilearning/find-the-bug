## Πρώτο επίπεδο

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![Το υπόβαθρο του Spotlight με ένα έντομο.](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

Πρόσθεσε το υπόβαθρο **Spotlight** από την κατηγορία **Μουσική**.

![Το εικονίδιο 'Επιλέξτε Υπόβαθρο'.](images/backdrop-button.png)

--- /task ---

### Resize the bug

--- task ---

Κάνε κλικ στο αντικείμενο **bug** στη λίστα αντικειμένων. Πρόσθεσε ένα script για να αλλάξεις το `μέγεθος`{:class="block3looks"} του εντόμου `όταν το υπόβαθρο αλλάζει σε Spotlight`{:class="block3events"}:

![Το αντικείμενο bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

Κάνε κλικ στον κώδικα για να αλλάξεις το μέγεθος και, στη συνέχεια, σύρε το μικροσκοπικό σου έντομο σε μια κρυψώνα.

Πρόσθεσε κώδικα για να τοποθετήσεις το έντομό σου:

![Το αντικείμενο bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Επίλεξε:** Μπορείς να επιλέξεις διαφορετικό μέγεθος και τοποθεσία, αν προτιμάς.

--- /task ---

### Move to the next Backdrop

Όταν παίζεις το παιχνίδι και βρεις με επιτυχία το έντομο, το παιχνίδι θα αλλάξει στο επόμενο υπόβαθρο. Επίσης, για να ξεκινήσεις το παιχνίδι, θα κάνεις κλικ στο έντομο στην οθόνη 'start'.

Το μπλοκ `επόμενο υπόβαθρο`{:class="block3looks"} αλλάζει στο επόμενο υπόβαθρο με τη σειρά με την οποία εμφανίζονται τα υπόβαθρα όταν κάνεις κλικ στην καρτέλα **Υπόβαθρα** στην **Σκηνή**.

--- task ---

Πρόσθεσε ένα script στο αντικείμενο σου **bug** για να `παίξει τον ήχο Pop`{:class="block3sound"} και πήγαινε στο `επόμενο υπόβαθρο`{:class="block3looks"} `όταν γίνει κλικ σε αυτό το αντικείμενο`{:class ="block3events"}:

![Το αντικείμενο bug.](images/bug-sprite.png)

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
title: Δεν συμβαίνει τίποτα όταν κάνω κλικ στο έντομο
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---