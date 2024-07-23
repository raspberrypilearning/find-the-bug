--- question ---
---
legend: Frage 2 von 3
---

Du hast eine `wiederhole fortlaufend`{:class="block3control"}-Schleife verwendet, um die Figur **Papagei** auf lästige Weise herumfliegen zu lassen.

Wir haben versucht, eine weitere Ablenkungsfigur hinzuzufügen, aber sie bewegt sich nur einmal, wenn wir auf die grüne Flagge klicken, und stoppt dann. Wie können wir das beheben?

![Die Raketenfigur.](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [all around v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [color v] effect by [25] 
wait [0.5] seconds 
end
```

--- choices ---

- ( ) Ändere die Zahl im Block `gehe`{:class="block3motion"}

  --- feedback ---

Wenn du die Zahl im Block `gehe`{:class="block3motion"} änderst, veränderst du, wie weit sich die Figur bewegt, wenn auf die grüne Flagge geklickt wird. Aber diese Änderung bewirkt nicht, dass die Rakete sich weiter bewegt.

  --- /feedback ---

- ( ) Entferne den `pralle vom Rand ab`{:class="block3motion"}-Block

  --- feedback ---

Der Block `pralle vom Rand ab`{:class="block3motion"} lässt die Figur vom Rand der Bühne abprallen. Wenn du es entfernen würdest, würde die Rakete am Rand der Bühne stecken bleiben.

  --- /feedback ---

- ( ) Füge einen weiteren `wiederhole fortlaufend`{:class="block3control"}-Block hinzu

--- feedback ---

Ein Skript kann nur einen `wiederhole fortlaufend`{:class="block3control"}-Block haben. Ist dir aufgefallen, dass du keinen Block unter einem Block `wiederhole fortlaufend`{:class="block3control"} hinzufügen kannst?

--- /feedback ---

- (x) Ziehe den Block `gehe`{:class="block3motion"} in die `wiederhole fortlaufend`{:class="block3control"}-Schleife

  --- feedback ---

  Ja! Die Figur bewegt sich nur einmal. Wenn du den `gehe`{:class="block3motion"}- Block innerhalb der`wiederhole fortlaufend`{:class="block3control"}- Schleife verschiebst, wird sich die Figur bewegen, bis du dein Projekt beendest.

  --- /feedback ---

--- /choices ---

--- /question ---
