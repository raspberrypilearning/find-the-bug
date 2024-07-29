## Verbessere dein Spiel

Wenn du Zeit hast, kannst du deinem Spiel weitere Level und mehr Ablenkungen hinzufügen. Du kannst auch die versteckte Figur und den Text auf der Tafel ändern.

--- task ---

Spiele dein Spiel und schau mal, wie schnell du die Bugs finden kannst.

Gibt es noch jemanden, der dein Spiel ausprobieren kann? Wie schnell können sie die Bugs finden? Sie wissen nicht, wo du sie versteckt hast, daher kann es etwas länger dauern!

Gibt es etwas, das du ändern möchtest?

Du könntest:
- Den Papagei noch nerviger machen
- Die Bugs kleiner machen
- Den `Effekt Farbe`{:class="block3looks"} ändern, um den Bug auf jedem Level zu tarnen
- Die Schriftart oder Farbe des Textes ändern

--- /task ---

### Füge weitere Level hinzu

--- task ---

Hier sind die Blöcke, die du benötigst, um den Bug auf einem neuen Level zu verstecken:

```blocks3
when backdrop switches to [neues Level v]

set size to [20] %

go to x: [0] y: [0] // ziehe den Bug um ihn zunächst zu positionieren

set [Farbe v] effect to [50]
```

Für jedes Level musst du:
- Ein Bühnenbild hinzufügen
- Auf den Bühnenbereich klicken, dann auf die Registerkarte **Hintergrundbilder** wechseln, und dann den neuen Hintergrund an die Position vor dem **'Ende'** Hintergrund ziehen
- Einen Block `wenn das Bühnenbild wechselt`{:class="block3events"} für den neuen Hintergrund hinzufugen, und Code schreiben, um den Bug zu positionieren und zu verbergen

**Tipp:** Um den Bug in ein neues Versteck zu ziehen, musst du den Code „unterbrechen“, damit der Hintergrund nicht wechselt, wenn du auf den Bug klickst, um ihn im neuen Level zu positionieren.

--- /task ---

### Füge weitere Ablenkungen hinzu

--- task ---

Du kannst weitere Papageien hinzufügen oder eine andere Figur auswählen, die als Ablenkung dient.

Hier ist der Code, den du für den Papagei verwendet hast:

```blocks3
when flag clicked
set rotation style [links-rechts v] // nicht umdrehen
point in direction [35] // Zahlen von -180 bis 180
forever // bleib nervig
move [10] steps // die Zahl kontrolliert die Geschwindigkeit
if on edge, bounce // bleib auf der Bühne
next costume // schlage die Flügel
change [Farbe v] effect by [5] // versuche 11 oder 50
wait [0.25] seconds // versuche 0.1 oder 0.5
end
```

**Tipp:** Du kannst den Code der **Papagei**-Figur auf eine andere Figur ziehen, um schneller eine neue Ablenkungsfigur erstellen.

![Code aus dem Codebereich in eine andere Figur in der Figurliste ziehen.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Abgeschlossenes Projekt
---

Du findest das [abgeschlossene Projekt hier](https://scratch.mit.edu/projects/1049403470/){:target="_blank"}.

--- /collapse ---