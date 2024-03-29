## Eindscherm

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Je gaat een 'eind' scherm maken om te laten zien hoeveel seconden de speler nodig had om de kevers te vinden. 
</div>
<div>

![De kever met de hoeveelheid tijd in een tekstballon.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Soms is alleen het verslaan van een spel niet genoeg. Spelers willen graag weten hoe ze het hebben gedaan tegen andere spelers of tegen zichzelf. Kun je een spel bedenken dat laat zien hoe goed je het hebt gedaan?</p>

### Voeg nog een achtergrond toe

--- task ---

Voeg de **Chalkboard** (bord) achtergrond uit de categorie **Binnen** toe.

![De Chalkboard achtergrond in de Achtergronden bibliotheek.](images/chalkboard.png)

**Tip:** In Scratch kun je dezelfde achtergrond meer dan één keer toevoegen.

--- /task ---

### Bewerk de achtergrond

--- task ---

Klik op het **Achtergronden** tabblad om de Teken-editor te openen.

![De Chalkboard achtergrond in de Teken-editor.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

Verander de naam van de achtergrond in `end` (einde):

![De achtergrondnaam is gewijzigd in de Teken-editor.](images/end-screen-name.png)

**Tip:** Je hernoemt je achtergrond naar **end** om je code makkelijker te begrijpen.

--- /task ---

### Positioneer de kever

--- task ---

Klik op de **kever** sprite en voeg code toe om de kever op het 'eind' scherm te plaatsen:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // volledige grootte
go to x: [0] y: [30] // op het bord
```

--- /task ---

### Voeg een klok toe

Hoeveel tijd kost het je om de kevers te vinden en erop te klikken? Scratch heeft een `klok`{:class="block3sensing"} die je hiervoor kunt gebruiken.

--- task ---

Het `klok`{:class="block3sensing"} blok komt uit het `Waarnemen`{:class="block3sensing"} blokkenmenu. Voeg code toe om de kever de `klok`{:class="block3sensing"} te laten `zeggen`{:class="block3looks"} op het 'eind' scherm:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // volledige grootte
go to x: [0] y: [30] // op het bord
+say (timer) // tijdsduur
```

![Een 'klok' blok toevoegen aan een 'zeg' blok.](images/inserting-blocks.gif)

--- /task ---

--- task ---

**Test:** Klik op de groene vlag om je zoekvaardigheid te testen. Hoeveel tijd kost het je om de kevers te vinden en erop te klikken?

--- /task ---

Om terug te gaan naar het 'start' scherm, klik je op de kever in het 'eind' scherm.

--- task ---

Voeg code toe om ervoor te zorgen dat de kever stopt met het zeggen van de `klok`{:class="block3sensing"} wanneer je naar het 'start' scherm gaat:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // volledige grootte
go to x: [0] y: [30] // op het bord
+say [] // zeg niets
```

--- /task ---

### Stop de klok

Als je het spel een tweede keer speelt, blijft de `klok`{:class="block3sensing"} tellen.

--- task ---

Voeg code toe om `zet klok op 0`{:class="block3sensing"} te doen wanneer de `achtergrond overschakelt naar`{:class="block3events"} het eerste niveau:

![De kever-sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // eerste niveau
set size to [20] % // klein
go to x: [13] y: [132] // op de discobal
+reset timer // start de klok
```

--- /task ---

--- task ---

**Test:** Klik op de groene vlag en speel het spel. De klok moet nu weer op 0 beginnen als je op de kever in het 'start' scherm klikt om naar het eerste niveau te gaan. Als je op de kever klikt in het 'eind' scherm, zou je terug moeten keren naar het 'start' scherm en zien dat de kever de `klok`{:class="block3sensing"} niet zegt.

--- /task ---

