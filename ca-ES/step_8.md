## Actualitza el teu joc

Si teniu temps, podeu afegir més nivells i més distraccions al vostre joc. També podeu canviar el personatge que s'amaga i canviar el text a la pissarra.

--- task ---

Juga al teu joc i mira amb quina rapidesa pots trobar els bitxos.

Hi ha algú més que pugui provar el teu joc? Amb quina rapidesa poden trobar els bitxos? No sabran on els has amagat, així que pot ser que triguin una mica més!

Hi ha alguna cosa que vulguis canviar?

Podríeu:
- Feu que el lloro sigui encara més molest
- Feu que els insectes siguin més petits
- Canvia l' `efecte de color`{:class="block3looks"} per camuflar el bitxo a cada nivell
- Canvia el tipus de lletra o el color del text

--- /task ---

### Afegeix més nivells

--- task ---

Aquests són els blocs que necessitareu per amagar el bitxo en un nou nivell:

```blocks3
when backdrop switches to [nou nivell v]

set size to [20] %

go to x: [0] y: [0] // arrossegueu per col·locar primer l'error

set [color v] effect to [50]
```

Per a cada nivell, haureu de:
- Afegir un fons
- Feu clic al panell de l'escenari, després a la pestanya **Fons** i arrossegueu el nou teló de fons a la posició abans del **fi** .
- Afegiu un bloc `següent fons de pantalla`{:class="block3events"} per al nou fons i afegiu codi a la posició, i amagueu el bitxo

**Consell:** Per arrossegar el bitxo a una nova posició oculta, haureu d'aturar el codi perquè el fons no canviï quan feu clic a bitxo, per deixar-ho a una nova posició al nou nivell.

--- /task ---

### Afegiu més distraccions

--- task ---

Podeu afegir més lloros o triar un altre personatges per actuar com a distracció.

Aquí teniu el codi que heu utilitzat per al lloro:

```blocks3
when flag clicked
set rotation style [esquerra-dreta v] // no vagis cap per avall
point in direction [35] // nombre de -180 a 180
forever // segueix sent molest
move [10] steps // el nombre que controla la velocitat
if on edge, bounce // romandre a l'escenari
next costume // solapa
change [color v] effect by [5] // prova 11 o 50
wait [0.25] seconds // prova 0,1 o 0,5
end
```

**Consell:** Podeu arrossegar el codi del personatge **Parrot** a un altre personatge perquè sigui més ràpid crear una altra distracció.

![Arrossegant codi des de l'àrea de codi a un altre personatge de la llista de Personatges.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Projecte finalitzat
---

Pots veure el [projecte completat  aquí](https://scratch.mit.edu/projects/1102897026/){:target="_blank"}.

--- /collapse ---