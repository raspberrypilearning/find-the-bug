--- question ---
---
legend: Domanda 2 di 3
---

Hai usato un ciclo `per sempre`{:class="block3control"} per far volare lo sprite **Parrot** in modo fastidioso.

Abbiamo provato ad aggiungere un altro sprite come distrazione, ma si muove solo una volta quando clicchiamo sulla bandierina verde e poi si ferma. Come possiamo aggiustarlo?

![Lo sprite Rocket.](images/rocket-sprite.png)

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

- ( ) Cambia il numero nel blocco `fai passi`{:class="block3motion"}

  --- feedback ---

Se cambi il numero nel blocco `fai passi`{:class="block3motion"}, cambierai la distanza in cui si muove lo sprite quando si fa clic sulla bandierina verde, ma questa modifica non farà muovere il razzo per sempre.

  --- /feedback ---

- ( ) Rimuovi il blocco `rimbalza quando tocchi il bordo`{:class="block3motion"}

  --- feedback ---

Il blocco `rimbalza quando tocchi il bordo`{:class="block3motion"} fa rimbalzare lo sprite sul bordo dello Stage. Se lo rimuovi, il razzo rimarrà bloccato sul bordo dello Stage.

  --- /feedback ---

- ( ) Aggiungi un altro blocco `per sempre`{:class="block3control"}

--- feedback ---

Uno script può avere solo un blocco `per sempre`{:class="block3control"}. Hai notato che non puoi aggiungere un blocco sotto un altro blocco `per sempre`{:class="block3control"}?

--- /feedback ---

- (x) Trascina il blocco `fai passi`{:class="block3motion"} all'interno del ciclo `per sempre`{:class="block3control"}

  --- feedback ---

  Sì! Lo sprite si muove solo una volta. Se sposti il blocco `fai passi`{:class="block3motion"} all'interno del ciclo `per sempre`{:class="block3control"}, lo sprite continuerà a muoversi finché non interrompi il progetto.

  --- /feedback ---

--- /choices ---

--- /question ---
