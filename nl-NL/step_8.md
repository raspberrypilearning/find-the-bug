## Verbeter je spel

Als je tijd hebt, kun je meer niveaus en meer afleidingen aan je spel toevoegen. Je kunt ook de sprite die zich verstopt en de tekst op het bord veranderen.

--- task ---

Speel je spel en kijk hoe snel je de kevers kunt vinden.

Is er iemand anders die jouw spel kan uitproberen? Hoe snel kunnen ze de kevers vinden? Ze zullen niet weten waar je ze hebt verstopt, dus het kan hen wat meer tijd kosten!

Is er iets dat je wilt veranderen?

Je kunt:
- De papegaai nog vervelender kunnen maken
- Maak de kever kleiner
- Het `kleur effect`{:class="block3looks"} veranderen om de kever op elk niveau te camoufleren
- Het lettertype of kleur van de tekst veranderen

--- /task ---

### Voeg meer niveaus toe

--- task ---

Dit zijn de blokken die je nodig hebt om een kever op een nieuw niveau te verstoppen:

```blocks3
when backdrop switches to [nieuw level v]

set size to [20] %

go to x: [0] y: [0] // versleep de kever eerst naar z'n positie

set [color v] effect to [50]
```

Voor elk niveau, moet je:
- Een achtergrond toevoegen
- Op het speelveld klikken, dan op het **Achtergronden** tabblad, en de nieuwe achtergrond dan naar de plaats vóór de **eind** achtergrond slepen
- Een `wanneer achtergrond verandert naar`{:class="block3events"} blok toevoegen voor de nieuwe achtergrond en code toevoegen om de kever te positioneren en te verstoppen

**Tip:** Om de kever naar een nieuwe verstopplek te slepen, moet je de code 'opbreken' zodat de achtergrond niet verandert als je op de kever klikt om een nieuwe positie te kiezen.

--- /task ---

### Voeg meer afleidingen toe

--- task ---

Je kunt meer papegaaien of andere sprites kiezen die zorgen voor afleiding.

Dit is de code die je gebruikt hebt voor de papegaai:

```blocks3
when flag clicked
set rotation style [left-right v] // draai niet ondersteboven
point in direction [35] // getal van -180 tot 180
forever // blijf vervelend doen
move [10] steps // het getal bepaalt de snelheid
if on edge, bounce // blijf op het speelveld
next costume // flapper
change [color v] effect by [5] // probeer 11 of 50
wait [0.25] seconds // probeer 0.1 of 0.5
end
```

**Tip:** Je kunt de code van de **Parrot** sprite verslepen naar een andere sprite om sneller een andere afleidingssprite te maken.

![Code verslepen van het werkgebied naar een andere sprite in de sprite lijst.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Voltooid project
---

Je kan het [voltooid project hier](https://scratch.mit.edu/projects/600272350/){:target="_blank"} bekijken.

--- /collapse ---