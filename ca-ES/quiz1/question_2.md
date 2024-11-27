--- question ---
---
legend: Pregunta 2 de 3
---

Has fet servir un bucle `per sempre`{:class="block3control"} per fer que el personatge **Parrot** volés d'una manera molesta.

Hem intentat afegir un altre personatge de distracció, però només es mou una vegada quan fem clic a la bandera verda i després s'atura. Com ho podem arreglar?

![El personatge d'en Rocket.](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [al voltant v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [color v] effect by [25] 
wait [0.5] seconds 
end
```

--- choices ---

- ( ) Canvieu el número al bloc `mou-te`{:class="block3motion"}

  --- feedback ---

Si canvieu el número al bloc `mou-te`{:class="block3motion"}, canviareu fins a quin punt es mou el personatge quan es faci clic a la bandera verda, però aquest canvi no farà que el coet segueix movent-se.

  --- /feedback ---

- ( ) Elimina el `si estàs a la vora, rebota el bloc`{:class="block3motion"}

  --- feedback ---

El `si està a la vora, rebota`{:class="block3motion"} fa que el personatge reboti a la vora de l'escenari. Si el traieu, el coet quedaria enganxat a la vora de l'escenari.

  --- /feedback ---

- ( ) Afegeix un altre bloc `per sempre`{:class="block3control"}

--- feedback ---

Una llista d'accions només pot tenir un bloc `per sempre`{:class="block3control"}. Us heu adonat que no podeu afegir un bloc sota un bloc `per sempre`{:class="block3control"}?

--- /feedback ---

- (x) Arrossegueu el bloc `mou-te`{:class="block3motion"} dins del bucle `per sempre`{:class="block3control"}

  --- feedback ---

  Sí! El personatge només es mou una vegada. Si moveu el `mou-te`{:class="block3motion"} dins del bucle `per sempre`{:class="block3control"}, el personatge continua en moviment fins que atureu el vostre projecte.

  --- /feedback ---

--- /choices ---

--- /question ---
