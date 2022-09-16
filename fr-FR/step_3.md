## Premier niveau

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![L'arrière-plan projecteur avec un bug.](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

Ajoute le **Spotlight** de la catégorie **Music**.

![L'icône « Choisir un arrière-plan ».](images/backdrop-button.png)

--- /task ---

### Resize the bug

--- task ---

Clique sur le sprite **bug** dans la liste Sprite. Ajoute un script pour changer la `taille`{:class="block3looks"} de ton bug `quand l'arrière-plan bascule sur projecteur`{:class="block3events"} :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

Clique sur le code pour changer la taille, puis fais glisser ton petit bug vers une cachette.

Ajoute du code pour positionner ton bug :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Choisir :** Tu peux choisir une taille et un emplacement différents, si tu préféres.

--- /task ---

### Move to the next Backdrop

Lorsque tu joues au jeu et que tu trouves le bug avec succès, le jeu passe à l'arrière-plan suivant. De plus, pour démarrer le jeu, tu devras cliquer sur le bug sur l'écran « début ».

Le bloc `arrière-plan suivant`{:class="block3looks"} passe au prochain arrière-plan dans l'ordre dans lequel les arrière-plans sont listés lorsque tu cliques sur l'onglet **arrière-plans** pour la **scène**.

--- task ---

Ajoute un script à ton sprite **bug** pour `jouer le son Pop`{:class="block3sound"} et passer à l'`arrière-plan suivant`{:class="block3looks"} `quand ce sprite est cliqué`{:class ="block3events"} :

![Le sprite bug.](images/bug-sprite.png)

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
title: Rien ne se passe quand je clique sur le bug
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---