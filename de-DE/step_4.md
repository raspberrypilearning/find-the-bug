## Ablenkung durch einen Papageien

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Um es Spielern zu erschweren, den Bug zu finden und anzuklicken, füge einen nervigen Papagei hinzu, um sie abzulenken. 
</div>
<div>

![Ein bunter Papagei auf der Bühne.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Add the Parrot sprite

--- task ---

Add the **Parrot** sprite.

![Das Symbol "Figur wählen".](images/sprite-button.png)

--- /task ---

### Animate the Parrot sprite

Im Projekt [Erwische den Bus](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"} hast Du eine `wiederhole`{:class="block3control"} Schleife verwendet.

Du wirst hier eine andere Schleife verwenden. Eine `wiederhole fortlaufend`{:class="block3control"} Schleife führt die darin enthaltenen Codeblöcke immer wieder aus. Es ist die perfekte Schleife für einen lästigen Papagei, der nicht aufhört, herumzufliegen und in die Quere zu kommen.

--- task ---

Füge Code hinzu, um den Papagei auf ablenkende Weise herumflattern zu lassen:

![The Parrot sprite.](images/parrot-sprite.png)


```blocks3
when flag clicked
set rotation style [left-right v] // do not go upside down
point in direction [35] // number from -180 to 180
forever // keep being annoying
move [10] steps // the number controls the speed
if on edge, bounce // stay on the Stage
next costume // flap
change [color v] effect by [5] // try 11 or 50
wait [0.25] seconds // try 0.1 or 0.5
end
```

--- /task ---

--- task ---

**Test:** Klicke auf die grüne Flagge und teste dein Projekt erneut. Kannst du dich erinnern, wo du den Käfer versteckt hast?

In Scratch leuchtet der ausgeführte Code mit einer gelben Umrandung:

![](images/running-code.png)

**Tipp:** Wenn der Papagei beim Programmieren zu nervig wird, kannst du auf die rote Stopp-Schaltfläche über der Bühne klicken, um die Ausführung des Codes zu stoppen.

--- /task ---

