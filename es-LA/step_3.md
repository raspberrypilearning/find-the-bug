## Primer nivel

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Agregarás un nuevo fondo como primer nivel en tu juego y ocultarás el error.
</div>
<div>

![El fondo Spotlight con un error.](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

Agrega el fondo **Spotlight** de la categoría **Música**.

![El icono 'Elige un fondo'.](images/backdrop-button.png)

--- /task ---

### Redimensiona el error

--- task ---

Haz clic en el objeto **insecto** en la lista de Objetos. Añade un script cambiar el `tamaño`{:class="block3looks"} de tu insecto `cuando el fondo cambie a Spotlight`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

Haz clic en el código para cambiar el tamaño, luego arrastra tu pequeño insecto a un escondite.

Añade código para posicionar tu insecto:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Elige:** Puedes elegir un tamaño y una ubicación diferentes, si lo prefieres.

--- /task ---

### Move to the next Backdrop

Cuando juegas y encuentras con éxito el insecto, el juego cambiará al siguiente fondo. Además, para iniciar el juego, harás clic en el error en la pantalla de "inicio".

El bloque `siguiente fondo`{:class="block3looks"} cambia al siguiente fondo en el orden en que se enumeran los fondos cuando haces clic en la pestaña **Fondos** para el **Escenario**.

--- task ---

Añade un script a tu objeto **insecto** para `reproducir un sonido Pop`{:class="block3sound"} y cambiar al `siguiente fondo`{:class="block3looks"} `al hacer clic en este objeto`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

### Make the game start with the Start Screen

--- task ---

Click on the Stage pane and add this code to the **Stage**:

![The Spotlight backdrop.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // 'start' screen
```

--- /task ---

--- task ---

**Prueba:** Haz clic en la bandera verde para probar tu proyecto.

Notarás que en la pantalla de 'inicio', el error aún tendrá la configuración para esconderse en su escondite del primer nivel (en este ejemplo, en la bola de discoteca).

**Consejo:** Después del último fondo de la lista, `siguiente fondo`{:class="block3looks"} volverá al primer fondo.

--- /task ---

--- task ---

Haz clic en el objeto **error** en la lista de Objetos. Añade un script para `fijar el tamaño`{:class="block3looks"} del error cuando tu `fondo cambia a`{:class="block3events"} la pantalla de `inicio`{:class="block3events"}:

![El objeto error.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
```

--- /task ---

### Cambia la posición del insecto

--- task ---

Intenta colocar el insecto en la pantalla de 'inicio'.

¡Tu código hará que el fondo cambie cuando hagas clic en el insecto! Eso no es útil cuando intentas posicionar el insecto.

Para solucionar el problema, debes detener la ejecución del código cuando hagas clic en el insecto.

--- /task ---

--- task ---

Click on the green flag to return to the 'start' screen.

Haz clic en el objeto **insecto** en la lista de Objetos y arrastra los bloques lejos del bloque `al hacer clic en este objeto`{:class="block3events"}:

![Breaking the script.](images/breaking-script.png)

--- /task ---

--- task ---

Intenta posicionar el insecto nuevamente. Arrastra el insecto a la pizarra, debajo del texto:

![El insecto en la pantalla de inicio](images/bug-chalkboard.png)

Añade código para asegurarte de que el insecto se posicione en la pizarra cada vez que tu `fondo cambia a`{:class="block3events"} la pantalla de `inicio`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

Join the blocks back together so that the code blocks are under the `when this sprite clicked`{:class="block3events"} block again:

![The 'when this sprite clicked' block joined to the 'play sound' and 'next backdrop' blocks.](images/fixed-script.png)

--- /task ---

--- task ---

**Prueba:** Haz clic en la bandera verde para probar tu proyecto. Haz clic en el insecto para pasar al siguiente fondo. El insecto debería ser grande en la pantalla de 'inicio' y pequeño en el nivel de 'Spotlight'.

--- collapse ---
---
title: No pasa nada cuando hago clic en el insecto
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---