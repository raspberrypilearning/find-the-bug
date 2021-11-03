## Segundo nivel

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Elegirás un fondo para crear un segundo nivel en tu juego y hacer que el insecto sea difícil de encontrar. 
</div>
<div>

![Una escena en la calle con un insecto oculto.](images/second-level.png){:width="300px"}

</div>
</div>

--- task ---

**Elige:** Elige un fondo para tu segundo nivel. Hemos elegido el fondo **Urban**, pero puedes elegir el que más te guste.

![](images/insert-urban-backdrop.png)

**Consejo:** Recuerda que los fondos con muchos colores y detalles harán que el insecto sea más difícil de encontrar. ¿Qué tan difícil harás tu juego?

--- /task ---

Para poder arrastrar tu insecto a una nueva posición, debes detener el script `al hacer clic en este objeto`{:class="block3events"} para que no se ejecute.

--- task ---

Arrastra los bloques lejos del bloque `al hacer clic en este objeto`{:class="block3events"} para evitar que se ejecuten cuando hagas clic en el insecto:

![](images/breaking-script.png)

--- /task ---

Tu insecto debe ser difícil de encontrar cuando el fondo cambia. Puedes cambiar el tamaño del insecto para que sea más difícil de encontrar.

--- task ---

Añade código a `fijar el tamaño`{: class = "block3looks"} del insecto para el segundo nivel:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Prueba:** Haz clic en tu nuevo script para ejecutarlo.

--- /task ---

--- task ---

Arrastra tu insecto en el escenario a un buen escondite para este nivel.

![El insecto escondido en el escaparate de la tienda en medio del fondo.](images/hidden-urban-backdrop.png)

--- /task ---

Posiciona el insecto en su escondite.

--- task ---

Agrega un bloque `ir a x: y:`{:class="block3motion"} a tu código:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

--- task ---

Vuelve a unir los bloques al bloque `al hacer clic en este objeto`{:class="block3events"} para que cuando se haga clic en el insecto, el fondo cambie al `siguiente fondo`{:class="block3looks"}:

![](images/fixed-script.png)

--- /task ---

--- task ---

**Prueba:** Haz clic en la bandera verde para probar tu proyecto.

--- /task ---

Tu insecto puede estar frente al loro ahora.

--- task ---

Añade un script para asegurarte de que tu insecto esté siempre `atrás`{: class = "block3looks"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Ahora, tu insecto siempre permanecerá atrás, incluso si necesitas cambiar su posición.

--- /task ---

--- save ---
