--- question ---
---
legend: Frage 3 von 3
---

Du hast dieses Skript zur **Bug**Figur hinzugefügt:

![Die Bug Figur.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

Wie lässt der `sage`{:class="block3looks"} `Stoppuhr`{:class="block3sensing"}-Block die Bühne aussehen, wenn der Hintergrund auf **Ende** wechselt?

--- choices ---

- ( ) ![Ein Papagei sagt die Stoppuhrzeit "4.52".](images/quiz_parrot_number.png)

  --- feedback ---

Schau dir das Skript noch einmal an und überlege, welche die Hauptfigur des Spiels ist (der Papagei ist nur eine lästige Ablenkung).

  --- /feedback ---

- ( ) ![Ein Papagei sagt das Wort "Stoppuhr".](images/quiz_parrot_timer.png)

  --- feedback ---

Der Block `Stoppuhr`{:class="block3sensing"} befindet sich im Blockmenü `Fühlen`{:class="block3sensing"}. Die Figur spricht nicht das Wort "Stoppuhr". Überlege auch, welche Figur diesen Code verwendet.

  --- /feedback ---

- (x) ![Ein Bug sagt die Stoppuhrzeit "4.52".](images/quiz_bug_number.png)

  --- feedback ---

Ja. Der Block `Stoppuhr`{:class="block3sensing"} meldet die Zeit seit Projektstart oder seit dem Zurücksetzen der Uhr. Der Block `sage`{:class="block3looks"} erzeugt eine Sprechblase neben dem Bug.

  --- /feedback ---

- ( ) ![Ein Bug sagt das Wort "Stoppuhr".](images/quiz_bug_timer.png)

  --- feedback ---

Der Block `Stoppuhr`{:class="block3sensing"} befindet sich im Blockmenü `Fühlen`{:class="block3sensing"}. Die Figur spricht nicht das Wort "Stoppuhr".

  --- /feedback ---

--- /choices ---

--- /question ---





