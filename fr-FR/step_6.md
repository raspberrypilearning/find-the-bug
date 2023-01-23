## Écran de fin

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Crée un écran de « fin » pour montrer le nombre de secondes qu'il a fallu au joueur pour trouver les bugs. 
</div>
<div>

![Le bug avec le temps passé dans une bulle de dialogue.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Parfois, seulement gagner une partie n'est pas suffisant. Les joueurs aiment savoir comment ils se sont comportés contre d'autres joueurs ou contre eux-mêmes. Peux-tu penser à un jeu qui te montre à quel point tu as bien fait ?</p>

### Ajouter un autre arrière-plan

--- task ---

Ajoute le **Chalkboard** de la catégorie **Indoors**.

![L'arrière-plan Chalkboard dans la bibliothèque des arrière-plans.](images/chalkboard.png)

**Astuce :** Dans Scratch, tu peux ajouter plusieurs fois le même arrière-plan.

--- /task ---

### Modifier l'arrière-plan

--- task ---

Clique sur l'onglet **arrière-plans** pour ouvrir l'éditeur de peinture.

![L'arrière-plan Chalkboard dans l'éditeur de peinture.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

Change le nom de l'arrière-plan en `fin`:

![Le nom de l'arrière-plan a changé dans l'éditeur de peinture.](images/end-screen-name.png)

**Astuce :** Tu renommes l'arrière-plan en **fin** pour faciliter la compréhension de ton code.

--- /task ---

### Positionner le bug

--- task ---

Clique sur le **bug** et ajoute du code pour positionner le bug sur l'écran de « fin » :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [fin v]
set size to [100] % // pleine grandeur
go to x: [0] y: [30] // sur le tableau
```

--- /task ---

### Ajouter un chronomètre

Combien de temps te faut-il pour trouver et cliquer sur les bugs ? Scratch a un `chronomètre`{:class="block3sensing"} que tu peux utiliser pour le découvrir.

--- task ---

Le bloc `chronomètre`{:class="block3sensing"} est dans le menu blocs `Capteurs`{:class="block3sensing"} . Ajoute du code pour que le bug `dise`{:class="block3looks"} le `chronomètre`{:class="block3sensing"} sur l'écran de « fin » :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [fin v]
set size to [100] % // pleine grandeur
go to x: [0] y: [30] // sur le tableau
+say (timer) // dire les secondes
```

![Insertion d'un bloc "chronomètre" dans un bloc "dire".](images/inserting-blocks.gif)

--- /task ---

--- task ---

**Test :** Clique sur le drapeau vert pour tester tes capacités de recherche. Combien de temps te faut-il pour trouver le bug ?

--- /task ---

Pour revenir à l'écran « début », clique sur le bug sur l'écran « fin ».

--- task ---

Ajoute du code pour que le bug arrête de dire le `chronomètre`{:class="block3sensing"} lorsque tu vas à l'écran « début » :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [début v]
set size to [100] % // pleine grandeur
go to x: [0] y: [30] // sur le tableau
+say [] // ne dis rien
```

--- /task ---

### Arrêter le chronomètre

Si tu joues au jeu une deuxième fois, le `chronomètre`{:class="block3sensing"} continuera à compter.

--- task ---

Ajoute le code `réinitialiser le chronomètre`{:class="block3sensing"}`quand l'arrière-plan bascule sur`{:class="block3events"} le premier niveau :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // premier niveau
set size to [20] % // minuscule
go to x: [13] y: [132] // sur la boule disco
+reset timer // démarrer le chronomètre
```

--- /task ---

--- task ---

**Test :** Clique sur le drapeau vert et lance le jeu. Le chronomètre devrait se réinitialiser lorsque tu cliques sur le bug sur l'écran « début » pour passer au premier niveau. Lorsque tu cliques sur le bug sur l'écran « fin », tu devrais revenir à l'écran « début » et voir que le bug ne dit pas le `chronomètre`{:class="block3sensing"}.

--- /task ---

