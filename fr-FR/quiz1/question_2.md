--- question ---
---
legend: Question 2 sur 3
---

Tu as utilisé une boucle `répéter indéfiniment`{:class="block3control"} pour faire voler le sprite **perroquet** d'une manière agaçante.

Nous avons essayé d'ajouter un autre sprite de distraction, mais il ne bouge qu'une fois lorsque nous cliquons sur le drapeau vert, puis s'arrête. Comment pouvons-nous résoudre cela ?

![Le sprite de fusée.](images/rocket-sprite.png)

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

- ( ) Modifie le nombre dans le bloc `avancer`{:class="block3motion"}

  --- feedback ---

Si tu modifies le nombre dans le bloc `avancer`{:class="block3motion"}, tu modifieras la distance de déplacement du sprite lorsque tu cliques sur le drapeau vert, mais ce changement ne fera pas que la fusée continue de se déplacer.

  --- /feedback ---

- ( ) Supprime le bloc `rebondir si le bord est atteint`{:class="block3motion"}

  --- feedback ---

Le bloc `rebondir si le bord est atteint`{:class="block3motion"} fait rebondir le sprite sur le bord de la scène. Si tu l’enlevais, la fusée resterait bloquée au bord de la scène.

  --- /feedback ---

- ( ) Ajoute un autre bloc `répéter indéfiniment`{:class="block3control"}

--- feedback ---

Un script ne peut avoir qu'un seul bloc `répéter indéfiniment`{:class="block3control"}. As-tu remarqué que tu ne peux pas ajouter de bloc sous un bloc `répéter indéfiniment`{:class="block3control"} ?

--- /feedback ---

- (x) Fait glisser le bloc `avancer`{:class="block3motion"} dans la boucle `répéter indéfiniment`{:class="block3control"}

  --- feedback ---

  Oui! Le sprite ne bouge qu'une seule fois. Si tu déplaces le bloc `avancer`{:class="block3motion"} à l'intérieur de la boucle `répéter indéfiniment`{:class="block3control"}, le sprite continuera de se déplacer jusqu'à ce que tu arrêtes ton projet.

  --- /feedback ---

--- /choices ---

--- /question ---
