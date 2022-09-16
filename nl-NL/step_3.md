## Eerste niveau

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![De Spotlight achtergrond met een kever.](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

Voeg de **Spotlight** (schijnwerpers) achtergrond uit de categorie **Binnen** toe.

![Het pictogram 'Kies een achtergrond'.](images/backdrop-button.png)

--- /task ---

### Resize the bug

--- task ---

Klik op de **kever** in het Sprite-venster. Voeg een script toe om de `grootte`{:class="block3looks"} van je kever te veranderen `wanneer de achtergrond verandert naar Spotlight`{:class="block3events"}:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

Klik op de code om de grootte te wijzigen en sleep vervolgens je kleine kever naar een schuilplaats.

Voeg code toe om je kever te positioneren:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Kies:** Je kunt een andere grootte en positie kiezen als je dat wilt.

--- /task ---

### Move to the next Backdrop

Wanneer je het spel speelt en je de kever vindt, schakelt het spel over naar de volgende achtergrond. Ook om het spel te starten, klik je op de kever in het 'start'-scherm.

Het `volgende achtergrond`{:class="block3looks"} blok schakelt over naar de volgende achtergrond in de volgorde van de lijst met achtergronden als je klikt op het **Achtergronden** tabblad voor het **Speelveld**.

--- task ---

Voeg een script toe aan je **kever** sprite om een `startgeluid`{:class="block3sound"} af te spelen en schakel over naar de `volgende achtergrond`{:class="block3looks"} `wanneer op deze sprite wordt geklikt`{:class ="blok3events"}:

![De kever-sprite.](images/bug-sprite.png)

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
title: Er gebeurt niets als ik op de kever klik
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---