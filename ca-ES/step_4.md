## Distracció del lloro

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Perquè sigui més difícil que els jugadors trobin i facin clic a bitxo, afegireu un lloro molest per distreure'ls. 
</div>
<div>

![Un lloro de colors a l'escenari.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Afegiu el personatge del  Lloro

--- task ---

Afegeix el personatge **Parrot** .

![La icona "Tria un Personatge".](images/sprite-button.png)

--- /task ---

### Anima el personatge del Lloro

Al projecte [Agafa el autobús](https://projects.raspberrypi.org/ca-ES/projects/catch-the-bus){:target="_blank"}, heu utilitzat un bucle `repeteix`{:class="block3control"}.

Aquí fareu servir un bucle diferent. Un bucle `per sempre`{:class="block3control"} executa els blocs de codi que hi ha dins una vegada i una altra. És el bucle perfecte per a un lloro molest que no deixarà de volar i d'interposar-se.

--- task ---

Afegiu el codi per fer que el lloro es mogui d'una manera que distregui. Mireu els comentaris sobre els blocs de codi per veure alguns números diferents per provar:

![El personatge del Lloro.](images/parrot-sprite.png)


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

--- /task ---

--- task ---

**Prova:** Feu clic a la bandera verda i torneu a provar el vostre projecte. Recordes on vas amagar el bitxo?

A Scratch, el codi que s'està executant brilla amb un contorn groc:

![](images/running-code.png)

**Consell:** Si el lloro es posa massa molest mentre esteu codificant, podeu fer clic al botó d'aturada vermell que hi ha a sobre de l'escenari per evitar que el codi s'executi.

--- /task ---

