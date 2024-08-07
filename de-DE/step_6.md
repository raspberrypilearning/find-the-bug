## Endbildschirm

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Erstelle einen Endbildschirm, um die Anzahl der Sekunden anzuzeigen, die der Spieler benötigt hat, um die Fehler zu finden. 
</div>
<div>

![Der Bug mit der Zeitdauer in einer Sprechblase.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Manchmal reicht es nicht aus, ein Spiel nur zu gewinnen. Spieler möchten gerne wissen, wie sie sich gegen andere Spieler oder gegen sich selbst geschlagen haben. Welches Spiel kennst du, das dir zeigt, wie gut du abgeschnitten hast?</p>

### Füge einen weiteren Hintergrund hinzu

--- task ---

Füge den Hintergrund **Chalkboard** aus der Kategorie **Innenräume** hinzu.

![Das Chalkboard Bühnenbild in der Hintergrundbibliothek.](images/chalkboard.png)

**Tipp:** In Scratch kannst du denselben Hintergrund mehrmals hinzufügen.

--- /task ---

### Bearbeite den Hintergrund

--- task ---

Klicke auf die Registerkarte **Hintergrundbilder**, um den Mal-Editor zu öffnen.

![Das Chalkboard Bühnenbild im Mal-Editor.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

Ändere den Namen des Hintergrundbilds in `Ende`:

![Der Name des Bühnenbildes wurde im Mal-Editor geändert.](images/end-screen-name.png)

**Tipp:** Du benennst den Hintergrund in **Ende** um, um das Verständnis deines Codes zu erleichtern.

--- /task ---

### Den Bug positionieren

--- task ---

Klicke auf die **Bug**-Figur und füge Code hinzu, um den Bug auf dem Endbildschirm zu positionieren:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Ende v]
set size to [100] % // volle Größe
go to x: [0] y: [30] // auf der Tafel
```

--- /task ---

### Eine Stoppuhr hinzufügen

Wie lange dauert es, den Bug zu finden und anzuklicken? Scratch verfügt über eine `Stoppuhr`{:class="block3sensing"}, mit dem du das herausfinden kannst.

--- task ---

Der Block `Stoppuhr`{:class="block3sensing"} befindet sich im Blockmenü `Fühlen`{:class="block3sensing"}. Füge Code hinzu, damit der Bug die `Zeit`{:class="block3sensing"} am „Ende“ Bildschirm `sagt`{:class="block3looks"}:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Ende v]
set size to [100] % // volle Größe
go to x: [0] y: [30] // auf der Tafel
+say (timer) // wieviele Sekunden gebraucht wurden
```

![Einfügen eines „Stoppuhr“-Blocks in einen „sage“-Block.](images/inserting-blocks.gif)

--- /task ---

--- task ---

**Test:** Klicke auf die grüne Flagge, um deine Suchkünste auf die Probe zu stellen. Wie lange dauert es, den Bug zu finden und anzuklicken?

--- /task ---

Um zum 'Start' Bildschirm zurückzukehren, klicke auf den Bug im 'Ende' Bildschirm.

--- task ---

Füge Code hinzu, damit der Bug aufhört, die `Stoppuhr`{:class="block3sensing"} anzuzeigen, wenn du zum 'Start' Bildschirm gehst:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Start v]
set size to [100] % // volle Größe
go to x: [0] y: [30] // auf der Tafel
+say [] // sag nichts
```

--- /task ---

### Halte die Stoppuhr an

Wenn du das Spiel ein zweites Mal spielst, zählt die `Stoppuhr`{:class="block3sensing"} weiter.

--- task ---

Füge Code hinzu, um `die Stoppuhr zurückzusetzen`{:class="block3sensing"}, `wenn das Bühnenbild zum`{:class="block3events"} ersten Level wechselt:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // erstes Level
set size to [20] % // winzig
go to x: [13] y: [132] // auf der Discokugel
+reset timer // starte die Stoppuhr
```

--- /task ---

--- task ---

**Test:** Klicke auf die grüne Flagge und spiele das Spiel. Die Stoppuhr sollte zurückgesetzt werden, wenn du auf dem Startbildschirm auf den Bug klickst, um zum ersten Level zu gelangen. Wenn du auf dem „Ende“ Bildschirm auf den Bug klickst, solltest du zum „Start“ Bildschirm zurückkehren und sehen, dass der Bug die `Stoppuhr`{:class="block3sensing"} nicht anzeigt.

--- /task ---

