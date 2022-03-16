--- question ---
---
legend: Vraag 2 van 3
---

Je hebt een `herhaal`{:class="block3control"} lus gebruikt om de **Parrot** (papegaai) sprite op een vervelende manier rond te laten vliegen.

We hebben geprobeerd nog een afleidingssprite toe te voegen, maar deze beweegt maar één keer wanneer we op de groene vlag klikken en stopt dan. Hoe kunnen we dat oplossen?

![De Rocket (raket) sprite.](images/rocket-sprite.png)

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

- ( ) Wijzig het getal in het `neem stappen`{:class="block3motion"} blok

  --- feedback ---

Als je het getal in het `neem stappen`{:class="block3motion"} verandert, verander je hoe ver de sprite beweegt wanneer op de groene vlag wordt geklikt, maar deze wijziging zorgt er niet voor dat de raket blijft bewegen.

  --- /feedback ---

- ( ) Verwijder het `keer om aan de rand`{:class="block3motion"} blok

  --- feedback ---

Het `keer om aan de rand`{:class="block3motion"} blok zorgt ervoor dat de sprite van de rand van het speelveld stuitert. Als je het zou verwijderen, zou de raket vast komen te zitten aan de rand van het speelveld.

  --- /feedback ---

- ( ) Voeg nog een `herhaal`{:class="block3control"} blok toe

--- feedback ---

Een script kan maar één `herhaal`{:class="block3control"} blok hebben. Is het je opgevallen dat je geen blok kunt toevoegen onder een `herhaal`{:class="block3control"} blok?

--- /feedback ---

- (x) Sleep het `neem stappen`{:class="block3motion"} blok binnen de `herhaal`{:class="block3control"} lus

  --- feedback ---

  Ja! De sprite beweegt maar één keer. Als je het `neem stappen`{:class="block3motion"} blok binnen de `herhaal`{:class="block3control"} lus zet, zal de sprite blijven bewegen totdat je je project stopt.

  --- /feedback ---

--- /choices ---

--- /question ---
