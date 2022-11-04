## Deuxième niveau

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Choisis un arrière-plan pour créer un deuxième niveau pour ton jeu et rendre le bug difficile à trouver. 
</div>
<div>

![Une scène de rue avec un bug caché.](images/second-level.png){:width="300px"}

</div>
</div>

### Ajouter un autre arrière-plan

--- task ---

**Choisir :** Choisis un arrière-plan pour ton deuxième niveau. Nous avons choisi l'arrière-plan **Urban** , mais tu peux choisir celui qui te plaît le plus.

![Le bug et le perroquet sur l'arrière-plan urbain.](images/insert-urban-backdrop.png)

**Astuce :** N'oublie pas que les arrière-plans avec beaucoup de couleurs et de détails rendront le bug plus difficile à trouver. À quel point vas-tu rendre ton jeu difficile ?

--- /task ---

### Arrêter l'exécution du code

--- task ---

Fais glisser les blocs à l'écart du bloc `quand ce sprite est cliqué` pour les empêcher de s'exécuter lorsque tu cliques sur le bug :

![Briser le code.](images/breaking-script.png)

--- /task ---

### Redimensionner le bug

--- task ---

Ajoute du code à `mettre la taille`{:class="block3looks"} du bug pour le deuxième niveau :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Test :** Clique sur ton nouveau script pour l'exécuter.

--- /task ---

### Cacher ton bug

--- task ---

Fais glisser ton bug sur la scène vers une bonne cachette pour ce niveau.

![Le bug caché dans la vitrine au milieu de l'arrière-plan.](images/hidden-urban-backdrop.png)

--- /task ---

Place ton bug dans sa cachette.

--- task ---

Ajoute un bloc `aller à x: y:`{:class="block3motion"} à ton code :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

### Tester ton code

--- task ---

Joins les blocs au bloc `quand ce sprite est cliqué`{:class="block3events"} afin que lorsque le bug est cliqué, l'arrière-plan bascule sur `l'arrière-plan suivant`{:class="block3looks"} :

![Les blocs sont réunis.](images/fixed-script.png)

--- /task ---

--- task ---

**Test :** Clique sur le drapeau vert pour tester ton projet.

--- /task ---

Ton bug peut être maintenant devant le perroquet.

--- task ---

Ajoute un script pour t'assurer que ton bug est toujours à l'`arrière`{:class="block3looks"} :

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Désormais, ton bug restera toujours à l'arrière, même si tu dois changer sa position.

--- /task ---
