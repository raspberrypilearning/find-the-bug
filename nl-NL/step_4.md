## Papegaai afleiding

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Om het voor spelers moeilijker te maken om de kever te vinden en erop te klikken, voeg je een vervelende papegaai toe om ze af te leiden. 
</div>
<div>

![Een kleurrijke papegaai op het speelveld.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

--- task ---

Voeg de **Parrot** (papegaai) sprite toe.

![Het pictogram 'Kies een Sprite'.](images/sprite-button.png)

--- /task ---

In het [Neem de bus](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"}-project heb je een `herhaal`{:class="block3control"} blok gebruikt.

Je gebruikt hier een andere lus. Een `herhaal`{:class="block3control"} lus voert de codeblokken daarbinnen keer op keer uit. Het is de perfecte lus voor een vervelende papegaai die niet stopt met rondvliegen en in de weg zitten.

--- task ---

Voeg code toe om de papegaai op een afleidende manier te laten fladderen:

![De Parrot sprite.](images/parrot-sprite.png)


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

**Test:** Klik op de groene vlag en test jouw project. Weet je nog waar je de kever verstopt hebt?

In Scratch heeft de code die uitgevoerd wordt een gele omtrek:

![](images/running-code.png)

**Tip:** Als de papegaai tijdens het coderen te vervelend wordt, kun je op de rode stop knop boven het speelveld klikken om te voorkomen dat de code wordt uitgevoerd.

--- /task ---

--- save ---