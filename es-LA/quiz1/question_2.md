--- question ---
---
legend: Pregunta 2 de 3
---

Usaste un bucle `por siempre`{:class="block3control"} para hacer que el objeto **Parrot** vuele de una manera molesta.

Hemos intentado agregar otro objeto de distracción, pero solo se mueve una vez cuando hacemos clic en la bandera verde y luego se detiene. ¿Cómo podemos solucionarlo?

![El objeto cohete.](images/rocket-sprite.png)

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

- ( ) Cambia el número en el bloque `mover`{:class="block3motion"}

  --- feedback ---

Si cambias el número en el bloque `mover`{:class="block3motion"}, cambiarás la distancia que se mueve el objeto al hacer clic en la bandera verde, pero este cambio no hará que el cohete siga moviéndose.

  --- /feedback ---

- () Elimina el bloque `si toca un borde, rebotar`{:class="block3motion"}

  --- feedback ---

El bloque `si toca un borde, rebotar`{:class="block3motion"} hace que el objeto rebote en el borde del escenario. Si lo quitaras, el cohete se atascaría en el borde del escenario.

  --- /feedback ---

- () Agrega otro bloque `por siempre`{:class="block3control"}

--- feedback ---

Un script solo puede tener un bloque `por siempre`{:class="block3control"}. ¿Notaste que no puedes agregar un bloque debajo de un bloque `por siempre`{:class="block3control"}?

--- /feedback ---

- (x) Arrastra el bloque `mover`{:class="block3motion"} dentro del bucle `por siempre`{:class="block3control"}

  --- feedback ---

  ¡Sí! El objeto solo se mueve una vez. Si mueves el bloque `mover`{:class="block3motion"} dentro del bucle `por siempre`{:class="block3control"}, el objeto seguirá moviéndose hasta que detengas tu proyecto.

  --- /feedback ---

--- /choices ---

--- /question ---
