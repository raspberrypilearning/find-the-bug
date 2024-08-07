## Erstes Level

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Füge als erstes Level in deinem Spiel ein neues Hintergrundbild hinzu und verberge den Bug.
</div>
<div>

![Der Spotlight Hintergrund mit einem Bug.](images/first-level.png){:width="300px"}

</div>
</div>

### Füge einen weiteren Hintergrund hinzu

--- task ---

Füge den Hintergrund **Spotlight** aus der Kategorie **Musik** hinzu.

![Das Symbol "Hintergrundbild wählen".](images/backdrop-button.png)

--- /task ---

### Ändere die Größe des Bugs

--- task ---

Klicke in der Figurenliste auf die **Bug**-Figur. Füge ein Skript hinzu, um die `Größe`{:class="block3looks"} deines Bugs zu ändern, `wenn das Bühnenbild zu Spotlight wechselt`{:class="block3events"}:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // winzig
```

--- /task ---

--- task ---

Klicke auf den Code, um die Größe zu ändern, und ziehe dann deinen kleinen Käfer in ein Versteck.

Füge Code hinzu, um deinen Bug zu positionieren:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // winzig
+ go to x: [13] y: [132] // auf der Discokugel
```

**Wähle:** Wenn du willst, kannst du eine andere Größe und eine andere Stelle wählen.

--- /task ---

### Gehe zum nächsten Hintergrundbild

Wenn du das Spiel spielst und den Bug erfolgreich findest, wechselt das Spiel zum nächsten Hintergrundbild. Und: um das Spiel zu starten, klickst du den Bug auf dem Startbildschirm.

Der Block `wechsle zum nächsten Bühnenbild`{:class="block3looks"} schaltet auf das nächste Bühnenbild in der Reihenfolge, in der die Bühnenbilder im Tab **Hintergrundbilder** der **Bühne** aufgeführt sind.

--- task ---

Füge deiner **Bug**-Figur ein Skript hinzu, um `einen Pop Klang`{:class="block3sound"} abzuspielen, und `wechsel zum nächste Hintergrundbild`{:class="block3looks"} `wenn diese Figur angeklickt wird`{:class="block3events"}:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

### Starte das Spiel mit dem Startbildschirm

--- task ---

Klicke auf den Bühnenbereich und füge diesen Code zur **Bühne**hinzu:

![Der Spotlight-Hintergrund.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [Start v] // 'start' Bildschirm
```

--- /task ---

--- task ---

**Test:** Klicke auf die grüne Flagge, um dein Projekt zu testen.

Du wirst feststellen, dass der Bug auf dem 'start' Bildschirm immer noch die Einstellungen hat, sich in seinem Versteck aus dem ersten Level zu verstecken (in diesem Beispiel auf der Discokugel).

**Tipp:** Nach dem letzten Hintergrundbild in der Liste wechselt `wechsle zum nächsten Bühnenbild`{:class="block3looks"} zurück zum ersten Hintergrundbild.

--- /task ---

--- task ---

Klicke in der Figurenliste auf die **Bug**-Figur. Füge ein Skript hinzu, das `die Größe des Bugs ändert`{:class="block3looks"}, `wenn das Bühnenbild zum`{:class="block3events"} `start`{:class="block3events"} Bildschirm wechselt:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Start v]
set size to [100] % // volle Größe
```

--- /task ---

### Ändere die Position des Bugs

--- task ---

Versuche, den Bug auf dem 'start' Bildschirm zu positionieren.

Dein Code bewirkt, dass das Hintergrundbild wechselt, wenn du auf den Bug klickst! Das ist nicht hilfreich, wenn du versuchst, den Bug zu positionieren.

Um das Problem zu beheben, musst du die Ausführung des Codes stoppen, wenn du auf den Bug klickst.

--- /task ---

--- task ---

Klicke auf die grüne Flagge, um zum 'start' Bildschirm zurückzukehren.

Klicke in der Figurenliste auf die Figur **bug** und ziehe die Blöcke vom Block `wenn diese Figur angeklickt wird`{:class="block3events"} weg:

![Das Skript trennen.](images/breaking-script.png)

--- /task ---

--- task ---

Versuch nochmal, den Käfer zu positionieren. Ziehe den Käfer auf die Tafel, unter den Text:

![Der Bug auf dem Startbildschirm](images/bug-chalkboard.png)

Füge Code hinzu, um sicherzustellen, dass der Bug jedes Mal auf der Tafel positioniert wird, `wenn das Bühnenbild zu`{:class="block3events"} `start`{:class="block3events"} wechselt:

![Die Bug-Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Start v]
set size to [100] % // volle Größe
+ go to x: [0] y: [30] // auf der Tafel
```

--- /task ---

--- task ---

Füge die Blöcke wieder zusammen, sodass die Codeblöcke erneut unter dem Block `wenn diese Figur angeklickt wird`{:class="block3events"} liegen:

![Der Block „Wenn diese Figur angeklickt wird“ ist mit den Blöcken „spiele Klang“ und „wechsle zum nächsten Bühnenbild“ verbunden.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Klicke auf die grüne Flagge, um dein Projekt zu testen. Klick auf den Bug, um zum nächsten Hintergrundbild zu gelangen. Der Bug sollte auf dem 'start' Bildschirm groß und auf dem 'Spotlight' Level klein sein.

--- collapse ---
---
title: Es passiert nichts, wenn ich auf den Bug klicke
---

Hast du vergessen, den Code wieder mit dem Block `wenn diese Figur angeklickt wird`{:class="block3events"} zu verbinden?

--- /collapse ---

--- /task ---