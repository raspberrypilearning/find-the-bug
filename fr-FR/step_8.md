## Améliorer ton jeu

Si tu as le temps, tu peux ajouter plus de niveaux et plus de distractions à ton jeu. Tu peux également changer le sprite qui se cache et changer le texte au tableau.

--- task ---

Joue ton jeu et vois à quelle vitesse tu peux trouver les bugs.

Y a-t-il quelqu'un d'autre qui peut essayer ton jeu ? À quelle vitesse peuvent-ils trouver les bugs ? Ils ne sauront pas où tu les as cachés, donc cela peut leur prendre un peu plus de temps !

Y a-t-il quelque chose que tu veux changer ?

Tu pourrais :
- Rendre le perroquet encore plus ennuyeux
- Réduire la taille des bugs
- Changer l'`effet couleur`{:class="block3looks"} pour camoufler le bug à chaque niveau
- Changer la police ou la couleur du texte

--- /task ---

### Ajouter plus de niveaux

--- task ---

Voici les blocs dont tu auras besoin pour cacher le bug à un nouveau niveau :

```blocks3
when backdrop switches to [nouveau niveau v]

set size to [20] %

go to x: [0] y: [0] // fais glisser pour positionner le bug en premier

set [color v] effect to [50]
```

Pour chaque niveau, tu devras :
- Ajouter un arrière-plan
- Cliquer sur le panneau Scène, puis sur l'onglet **Arrière-plans**, ensuite faire glisser le nouvel arrière-plan en position avant l'arrière-plan **fin**
- Ajouter un bloc `quand l'arrière-plan bascule sur`{:class="block3events"} pour le nouvel arrière-plan et ajouter du code pour positionner et cacher le bug

**Astuce :** Pour faire glisser le bug vers une nouvelle position cachée, tu devras « casser » le code afin que l'arrière-plan ne change pas lorsque tu cliques sur le bug pour le positionner à un nouveau niveau.

--- /task ---

### Ajouter plus de distractions

--- task ---

Tu peux ajouter plus de perroquets ou choisir un autre sprite pour faire office de distraction.

Voici le code que tu as utilisé pour le perroquet :

```blocks3
when flag clicked
set rotation style [left-right v] // ne va pas à l'envers
point in direction [35] // nombre de -180 à 180
forever // continue d'être ennuyeux
move [10] steps // le nombre contrôle la vitesse
if on edge, bounce // rester sur la scène
next costume // rabat
change [color v] effect by [5] // essayer 11 ou 50
wait [0.25] seconds // essayer 0.1 ou 0.5
end
```

**Astuce :** Tu peux faire glisser le sprite **Parrot** vers un autre sprite pour accélérer la création d'un autre sprite de distraction.

![Faire glisser le code de la zone Code vers un autre sprite dans la liste Sprite.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Le projet terminé
---

Tu peux voir le [projet terminé ici](https://scratch.mit.edu/projects/600265078/){:target="_blank"}.

--- /collapse ---