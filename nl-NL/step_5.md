## Tweede niveau

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Kies een achtergrond om een tweede niveau voor je spel te maken en zorg dat de kever moeilijk te vinden is. 
</div>
<div>

![Een straatbeeld met een verborgen kever.](images/second-level.png){:width="300px"}

</div>
</div>

### Voeg nog een achtergrond toe

--- task ---

**Kies:** Kies een achtergrond voor je tweede niveau. We hebben de **Urban** (stedelijk) achtergrond gekozen, maar je kunt degene kiezen die jij het leukst vindt.

![De kever en de papegaai op een stedelijke achtergrond.](images/insert-urban-backdrop.png)

**Tip:** Onthoud dat achtergronden met veel kleuren en details het moeilijker maken om de kever te vinden. Hoe moeilijk ga jij je spel maken?

--- /task ---

### Stop het uitvoeren van de code

--- task ---

Sleep de blokken weg van het `wanneer op deze sprite wordt geklikt`{:class="block3events"} blok om te voorkomen dat ze worden uitgevoerd wanneer je op de kever klikt:

![De code opbreken.](images/breaking-script.png)

--- /task ---

### Pas het formaat van de kever aan

--- task ---

Voeg code toe aan `maak grootte`{:class="block3looks"} voor de kever van het tweede niveau:

![De bug-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Test:** Klik op je nieuwe script om het uit te voeren.

--- /task ---

### Verberg je kever

--- task ---

Sleep je kever op het speelveld naar een goede verstopplek op dit niveau.

![De kever verstopt in de etalage in het midden van de achtergrond.](images/hidden-urban-backdrop.png)

--- /task ---

Plaats je kever in zijn verstopplek.

--- task ---

Voeg een `ga naar x: y:`{:class="block3motion"} blok toe:

![De bug-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

### Test je code

--- task ---

Voeg de blokken weer toe aan het `wanneer op deze sprite wordt geklikt`{:class="block3events"} blok zodat wanneer op de kever wordt geklikt de achtergrond overschakelt naar de `volgende achtergrond`{:class="block3looks"}:

![De blokken zijn weer samengevoegd.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Klik op de groene vlag om je project te testen.

--- /task ---

Je kever kan nu vóór de papegaai zitten.

--- task ---

Voeg een script toe om ervoor te zorgen dat je kever altijd op de `achtergrond`{:class="block3looks"} zit:

![De bug-sprite.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Nu blijft je kever altijd achterin, zelfs als je zijn positie moet veranderen.

--- /task ---
